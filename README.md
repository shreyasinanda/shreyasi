<!DOCTYPE html><html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>AI Study Helper</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            padding: 20px;
        }
        textarea {
            width: 80%;
            height: 100px;
        }
        #response {
            margin-top: 20px;
            font-weight: bold;
        }
    </style>
</head>
<body>
    <h1>AI Study Helper</h1>
    <h2>Summarization Tool</h2>
    <textarea id="textInput" placeholder="Enter text to summarize..."></textarea>
    <br>
    <button onclick="summarizeText()">Summarize</button>
    <p id="response"></p><h2>Chat with AI</h2>
<input type="text" id="chatInput" placeholder="Ask something...">
<button onclick="chatWithAI()">Send</button>
<p id="chatResponse"></p>

<script>
    function summarizeText() {
        let text = document.getElementById("textInput").value;
        document.getElementById("response").innerText = "Summarized: " + text.substring(0, 50) + "...";
    }
    
    function chatWithAI() {
        let userInput = document.getElementById("chatInput").value;
        document.getElementById("chatResponse").innerText = "AI: " + (userInput ? "That's an interesting question!" : "Please enter a question.");
    }
</script>

</body>
</html>
