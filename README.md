# crypto-ctf-challange-01
├── <!DOCTYPE html>
<html>
<head>
    <title>Crypto CTF Challenge</title>
    <link rel="stylesheet" href="static/styles.css">
</head>
<body>
    <div class="container">
        <h1>Crypto CTF Challenge</h1>
        <p>Solve the puzzle and submit the correct flag.</p>

        <h2>Challenge</h2>
        <p>Decode this:</p>

        <pre>U2FsdGVkX1+5FZP5VilYQmFyYW5nZQ==</pre>

        <h2>Submit Flag</h2>
        <input id="flagInput" placeholder="flag{your_answer}">
        <button onclick="checkFlag()">Submit</button>

        <p id="result"></p>
    </div>

    <script src="static/script.js"></script>
</body>
</html>
├── challenge/
│   ├──  
The text is encoded. Your task is to decode it and find the hidden fruit.

Flag format: flag{fruit_name}
│   ├── U2FsdGVkX1+5FZP5VilYQmFyYW5nZQ==
│   └── hint.txt
├── static/
│   ├──body {
    font-family: Arial;
    background: #0d0d0d;
    color: white;
    text-align: center;
}

.container {
    margin-top: 80px;
}

input {
    padding: 10px;
    width: 250px;
}
button {
    padding: 10px 20px;
    cursor: pointer;
}
│   └── function checkFlag() {
    let userFlag = document.getElementById("flagInput").value;
    let correct = "flag{orange}";

    if (userFlag === correct) {
        document.getElementById("result").innerHTML = "✅ Correct Flag!";
    } else {
        document.getElementById("result").innerHTML = "❌ Wrong Flag. Try again.";
    }
}
└── README.md
