<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Hacker's Blog</title>
    <style>
        body {
            background-color: #0d0d0d;
            color: #33ff33;
            font-family: "Courier New", Courier, monospace;
            text-align: center;
        }
        .container {
            max-width: 800px;
            margin: auto;
            padding: 20px;
        }
        h1 {
            border-bottom: 2px solid #33ff33;
            padding-bottom: 10px;
        }
        .post {
            background-color: #1a1a1a;
            padding: 15px;
            margin: 20px 0;
            border-radius: 5px;
            transition: transform 0.3s;
            cursor: pointer;
        }
        .post:hover {
            transform: scale(1.05);
        }
        .post h2 {
            color: #ff3333;
        }
        .footer {
            margin-top: 20px;
            font-size: 0.8em;
            color: #777;
        }
        .hidden {
            display: none;
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>Hacker's Blog</h1>
        
        <div class="post" onclick="toggleContent('post1')">
            <h2>Exploring Buffer Overflows</h2>
            <p class="hidden" id="post1">Understanding how buffer overflows work and how to exploit them...</p>
        </div>
        
        <div class="post" onclick="toggleContent('post2')">
            <h2>Top 10 Linux Commands for Pentesters</h2>
            <p class="hidden" id="post2">Essential Linux commands every penetration tester should know...</p>
        </div>
        
        <div class="post" onclick="toggleContent('post3')">
            <h2>Bypassing Firewalls with SSH Tunneling</h2>
            <p class="hidden" id="post3">A guide on how to use SSH tunneling to bypass network restrictions...</p>
        </div>
        
        <div class="footer">
            <p>&copy; 2025 Hacker's Blog | Stay Anonymous, Stay Secure</p>
        </div>
    </div>
    
    <script>
        function toggleContent(id) {
            var content = document.getElementById(id);
            content.classList.toggle("hidden");
        }
    </script>
</body>
</html>
