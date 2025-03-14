# YDOIDOTHIS.github.io
Allows searching on Apple Watch
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Apple Watch Search</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            background-color: black;
            color: white;
            padding: 10px;
        }
        input {
            width: 80%;
            padding: 8px;
            margin: 10px 0;
            font-size: 14px;
            text-align: center;
        }
        button {
            background-color: #1E90FF;
            color: white;
            border: none;
            padding: 10px 15px;
            font-size: 14px;
            cursor: pointer;
            border-radius: 5px;
        }
        button:hover {
            background-color: #0D74D9;
        }
    </style>
</head>
<body>
    <h2>Web Search</h2>
    <input type="text" id="searchQuery" placeholder="Enter search term">
    <button onclick="search()">Search</button>

    <script>
        function search() {
            let query = document.getElementById("searchQuery").value;
            if (query) {
                window.location.href = "https://www.google.com/search?q=" + encodeURIComponent(query);
            }
        }
    </script>
</body>
</html>
