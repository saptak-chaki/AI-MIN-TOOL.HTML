<!DOCTYPE html>
<html>
<body>
    <h1>AI Mini Tool</h1>
    <input type="text" id="userInput" placeholder="Ask something...">
    <button onclick="getResponse()">Submit</button>
    <p id="response"></p>

    <script>
        function getResponse() {
            const input = document.getElementById('userInput').value;
            document.getElementById('response').innerText = "AI says: You asked for '" + input + "'. This is a demo for the hackathon!";
        }
    </script>
</body>
</html>
