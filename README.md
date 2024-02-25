</html><head>
    <style>
        .animated-url {
            animation: marquee 5s linear infinite;
        }
    </style>
    <script>
        function loop() {
            var i, n, s = '';

            for (i = 0; i < 10; i++) {
                n = Math.floor(Math.sin((Date.now()/200) + (i/2)) * 4) + 4;

                s += String.fromCharCode(0x2581 + n);
            }

            window.location.hash = s;

            setTimeout(loop, 50);
        }

        loop();
    </script>
</head>
<body>
    <h1>Welcome to my website my name is David!</h1>
    <p>Check out this cool animated URL:</p>
    <form action="/action_page.php">
        <label for="fname">First name:</label><br>
        <input type="text" id="fname" name="fname"><br>
        <input type="submit" value="Submit">
    </form>
    <p class="animated-url">🌍🚀🌟https://www.example.com🌟🚀🌍</p>
</body>
</html>
</html>
