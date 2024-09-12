<!DOCTYPE html>
<html lang="de">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Online Ping Pong</title>
    <style>
        canvas {
            background: black;
            display: block;
            margin: 0 auto;
        }
        body {
            text-align: center;
            color: white;
            font-family: Arial, sans-serif;
        }
    </style>
</head>
<body>
    <h1>Online Ping Pong</h1>
    <canvas id="pongCanvas" width="600" height="400"></canvas>

    <script>
        const canvas = document.getElementById('pongCanvas');
        const ctx = canvas.getContext('2d');

        // Ball variables
        let ballX = canvas.width / 2;
        let ballY = canvas.height / 2;
        let ballRadius = 10;
        let ballSpeedX = 2;
        let ballSpeedY = 2;

        // Paddle variables
        const paddleWidth = 10;
        const paddleHeight = 75;
        const paddleSpeed = 5;

        // Left paddle
        let leftPaddleY = (canvas.height - paddleHeight) / 2;

        // Right paddle (AI)
        let rightPaddleY = (canvas.height - paddleHeight) / 2;

        // Input handling
        document.addEventListener('keydown', (event) => {
            if (event.key === 'ArrowUp' && leftPaddleY > 0) {
                leftPaddleY -= paddleSpeed;
            }
            if (event.key === 'ArrowDown' && leftPaddleY < canvas.height - paddleHeight) {
                leftPaddleY += paddleSpeed;
            }
        });

        // Draw the game
        function draw() {
            ctx.clearRect(0, 0, canvas.width, canvas.height);

            // Draw ball
            ctx.beginPath();
            ctx.arc(ballX, ballY, ballRadius, 0, Math.PI * 2);
            ctx.fillStyle = 'white';
            ctx.fill();
            ctx.closePath();

            // Draw left paddle
            ctx.fillRect(10, leftPaddleY, paddleWidth, paddleHeight);

            // Draw right paddle
            ctx.fillRect(canvas.width - paddleWidth - 10, rightPaddleY, paddleWidth, paddleHeight);

            // Move the ball
            ballX += ballSpeedX;
            ballY += ballSpeedY;

            // Ball collision with top/bottom walls
            if (ballY + ballRadius > canvas.height || ballY - ballRadius < 0) {
                ballSpeedY = -ballSpeedY;
            }

            // Ball collision with paddles
            if (
                ballX - ballRadius < 20 &&
                ballY > leftPaddleY &&
                ballY < leftPaddleY + paddleHeight
            ) {
                ballSpeedX = -ballSpeedX;
            }

            if (
                ballX + ballRadius > canvas.width - 20 &&
                ballY > rightPaddleY &&
                ballY < rightPaddleY + paddleHeight
            ) {
                ballSpeedX = -ballSpeedX;
            }

            // AI movement (simple follow the ball)
            if (rightPaddleY + paddleHeight / 2 < ballY) {
                rightPaddleY += paddleSpeed;
            } else if (rightPaddleY + paddleHeight / 2 > ballY) {
                rightPaddleY -= paddleSpeed;
            }

            // Reset ball if it goes off-screen
            if (ballX + ballRadius < 0 || ballX - ballRadius > canvas.width) {
                ballX = canvas.width / 2;
                ballY = canvas.height / 2;
                ballSpeedX = -ballSpeedX;
            }

            requestAnimationFrame(draw);
        }

        draw();
    </script>
</body>
</html>
