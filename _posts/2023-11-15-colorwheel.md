<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Binary Color Wheel</title>
    <style>
        body {
            display: flex;
            align-items: center;
            justify-content: center;
            height: 100vh;
            margin: 0;
        }
        canvas {
            border: 1px solid #000;
        }
    </style>
</head>
<body>
    <canvas id="colorWheel" width="400" height="400"></canvas>

    <script>
        const canvas = document.getElementById('colorWheel');
        const ctx = canvas.getContext('2d');

        const numSectors = 360;
        const radius = 150;
        const centerX = canvas.width / 2;
        const centerY = canvas.height / 2;

        function createBinaryColor(value) {
            const red = (value & 0b111111) << 2;
            const green = ((value >> 6) & 0b111111) << 2;
            const blue = ((value >> 12) & 0b111111) << 2;

            return `rgb(${red}, ${green}, ${blue})`;
        }

        function drawColorWheel() {
            for (let i = 0; i < numSectors; i++) {
                const angle = (i / numSectors) * (2 * Math.PI);
                const x = centerX + radius * Math.cos(angle);
                const y = centerY + radius * Math.sin(angle);

                const color = createBinaryColor(i);

                ctx.beginPath();
                ctx.moveTo(centerX, centerY);
                ctx.lineTo(x, y);
                ctx.strokeStyle = color;
                ctx.stroke();
            }
        }

        drawColorWheel();
    </script>
</body>
</html>
