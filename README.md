<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Valentine's Day Proposal</title> <!-- Change the title as needed -->
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background: linear-gradient(135deg, white, white);
            color: #333;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            overflow: hidden;
            position: relative;
        }
        .container {
            text-align: center;
            background: rgba(255, 182, 193, 0.9);
            padding: 20px;
            border-radius: 15px;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
            animation: fadeIn 2s ease-in-out;
        }
        h1 {
            font-size: 2.5em;
            color: #ff3366;
            animation: slideIn 1.5s ease-out;
            transition: transform 0.3s, color 0.3s;
        }
        h1:hover {
            transform: scale(1.1);
            color: #cc2952;
        }
        p {
            font-size: 1.2em;
            margin: 15px 0;
            animation: fadeUp 2s ease-out;
            transition: color 0.3s, transform 0.3s;
        }
        p:hover {
            color: #cc2952;
            transform: scale(1.05);
        }
        .btn-container {
            margin-top: 20px;
            animation: fadeIn 2.5s ease-in-out;
        }
        button {
            background: #ff3366;
            border: none;
            color: white;
            padding: 10px 20px;
            font-size: 1em;
            cursor: pointer;
            border-radius: 5px;
            transition: background 0.3s, transform 0.3s;
        }
        button:hover {
            background: #cc2952;
            transform: scale(1.1);
        }
        #response {
            margin-top: 20px;
            font-size: 1.5em;
            color: #2ecc71;
            animation: fadeIn 3s ease-in-out;
        }
    </style>
</head>
<body>
    <div class="container">
        <!-- Replace "Hannah" with another name if needed -->
        <h1>Hannah, Would you like to be my Valentine? 💖</h1>
        <p>Make this Valentine's Day special by saying yes!</p>
        <div class="btn-container">
            <button onclick="reply('Yes')">Yes</button>
            <button onclick="reply('No')">No</button>
        </div>
        <div id="response"></div>
        <div class="countdown" id="countdown"></div>
        <img src="https://media2.giphy.com/media/v1.Y2lkPTc5MGI3NjExYnoycGNoMXpid3h3dmtlODNsbGg5cWVhdXNiOXZsMGI5ZmtxOGE1NyZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9Zw/2PiRQ8JiAT22HSZpeW/giphy.gif" alt="Romantic GIF">
    </div>

    <script>
        function reply(answer) {
            const response = document.getElementById("response");
            const funnyResponses = [
                "I'll treat you some food!",  // Replace "Hannah" with another name if needed
                "aww pretty pleasee ://", // Replace "Hannah"
                "Don't say No! I'll handle the plans!",
                "pwease pwease, Hannah!", // Replace "Srijan"
                "aww me sadd :(( 💔 Please say yes!"
            ];

            if (answer === 'Yes') {
                response.textContent = "Yay! You've made my day, Hannah! 🥰"; // Replace "Srijan"
            } else {
                const randomResponse = funnyResponses[Math.floor(Math.random() * funnyResponses.length)];
                response.textContent = randomResponse;
            }
        }
    </script>
</body>
</html>
