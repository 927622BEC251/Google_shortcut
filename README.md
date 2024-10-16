# Google_shortcut
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Google Shortcut</title>
    <style>
        body {
            margin: 0;
            padding: 0;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            background: linear-gradient(135deg, #ff7e5f, #feb47b);
            font-family: 'Arial', sans-serif;
            animation: fadeInBg 2s ease-in-out;
        }

        @keyframes fadeInBg {
            from {
                opacity: 0;
            }
            to {
                opacity: 1;
            }
        }

        .container {
            text-align: center;
            background-color: white;
            padding: 40px;
            border-radius: 20px;
            box-shadow: 0px 10px 30px rgba(0, 0, 0, 0.2);
            animation: slideIn 1.5s ease-in-out;
        }

        @keyframes slideIn {
            from {
                transform: translateY(-50px);
                opacity: 0;
            }
            to {
                transform: translateY(0);
                opacity: 1;
            }
        }

        h1 {
            color: #4285f4;
            font-size: 3rem;
            margin-bottom: 20px;
            animation: bounceText 1.5s infinite;
        }

        @keyframes bounceText {
            0%, 100% {
                transform: translateY(0);
            }
            50% {
                transform: translateY(-10px);
            }
        }

        input {
            width: 300px;
            padding: 15px;
            font-size: 1.2rem;
            border-radius: 10px;
            border: 2px solid #ddd;
            margin-bottom: 20px;
            outline: none;
            transition: border-color 0.3s;
        }

        input:focus {
            border-color: #4285f4;
        }

        button {
            background-color: #4285f4;
            color: white;
            padding: 15px 30px;
            font-size: 1.2rem;
            border: none;
            border-radius: 10px;
            cursor: pointer;
            transition: transform 0.3s, background-color 0.3s;
        }

        button:hover {
            background-color: #357ae8;
            transform: scale(1.1);
        }

        button:active {
            transform: scale(0.95);
        }
    </style>
</head>
<body>

    <div class="container">
        <h1>Google Search</h1>
        <input type="text" id="searchQuery" placeholder="Search Google...">
        <br>
        <button onclick="searchGoogle()">Google Search</button>
    </div>

    <script>
        function searchGoogle() {
            const query = document.getElementById('searchQuery').value;
            if (query) {
                window.location.href = https://www.google.com/search?q=${query};
            } else {
                alert('Please enter a search query.');
            }
        }
    </script>

</body>
</html>
