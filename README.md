<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>AI Mini Tool</title>
    <style>
        body { font-family: sans-serif; display: flex; justify-content: center; align-items: center; height: 100vh; margin: 0; background-color: #f4f4f9; }
        .container { background: white; padding: 2rem; border-radius: 8px; box-shadow: 0 4px 6px rgba(0,0,0,0.1); text-align: center; }
        input { padding: 0.5rem; width: 250px; border: 1px solid #ccc; border-radius: 4px; }
        button { padding: 0.5rem 1rem; background-color: #007bff; color: white; border: none; border-radius: 4px; cursor: pointer; }
        button:hover { background-color: #0056b3; }
        #response { margin-top: 1rem; font-weight: bold; }
    </style>
</head>
<body>

<div class="container">
    <h1>AI Assistant Tool</h1>
    <p>Enter your query below:</p>
    <input type="text" id="userInput" placeholder="Ask something...">
    <button onclick="generateResponse()">Submit</button>
    <div id="response"></div>
</div>

<script>
    function generateResponse() {
        const input = document.getElementById('userInput').value;
        const responseDiv = document.getElementById('response');
        
        if (input.trim() === "") {
            responseDiv.innerText = "Please enter a valid query.";
            return;
        }

        // Logic to simulate AI response
        const responses = [
            "That's an interesting perspective!",
            "I'm still learning, but that sounds great.",
            "AI technology is evolving fast. Keep exploring!",
            "Great input! You are on the right track."
        ];
        const randomResponse = responses[Math.floor(Math.random() * responses.length)];
        
        responseDiv.innerText = "AI says: " + randomResponse;
    }
</script>

</body>
</html>
