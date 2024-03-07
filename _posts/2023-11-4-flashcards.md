---
toc: true
comments: true
layout: post
title: bio Flashcards
description: bio flashcards
type: hacks
courses: { compsci: {week: 11} }
---
<html>
<head>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f2e6ff; /* Light Purple background color */
            display: grid;
            place-items: center;
            min-height: 100vh;
        }

        /* Style for the question containers */
        .question-container {
            background-color: #fff;
            border-radius: 10px;
            box-shadow: 0 0 5px rgba(0, 0, 0, 0.2);
            max-width: 400px;
            margin: 10px;
            padding: 20px;
            text-align: left;
        }

        /* Style for question titles (changed font color to blue) */
        .question h2 {
            font-size: 18px;
            color: #3498db; /* Blue color for question titles */
        }

        /* Style for answer choices (changed font color to dark gray) */
        .question ul {
            list-style-type: none;
            padding: 0;
        }

        .question li {
            padding: 8px 0;
            color: #333; /* Dark gray color for answer choices */
        }

        /* Style for the correct answer reveal */
        .question details {
            margin-top: 15px;
            cursor: pointer;
        }

        .question summary {
            font-weight: bold;
            color: #333;
        }

        /* Style for the correct answer text color (changed to green) */
        .question details p {
            margin: 0;
            color: #009900; /* Green color for correct answer */
        }

        /* Arrange questions in two rows using grid layout */
        .questions-grid {
            display: grid;
            grid-template-columns: repeat(2, 1fr);
            gap: 20px;
        }
    </style>
</head>
<body>
    <div class="questions-grid">
        <div class="question-container">
            <div class="question">
                <h2>Biology Question 1</h2>
                <p>What is the powerhouse of the cell?</p>
                <ul>
                    <li>A) Nucleus</li>
                    <li>B) Mitochondria</li>
                    <li>C) Ribosome</li>
                    <li>D) Golgi apparatus</li>
                </ul>
                <details>
                    <summary>Click to reveal the correct answer</summary>
                    <p>The correct answer is B) Mitochondria</p>
                </details>
            </div>
        </div>

        <div class="question-container">
            <div class="question">
                <h2>Biology Question 2</h2>
                <p>Which gas do plants absorb from the atmosphere during photosynthesis?</p>
                <ul>
                    <li>A) Oxygen</li>
                    <li>B) Nitrogen</li>
                    <li>C) Carbon dioxide</li>
                    <li>D) Hydrogen</li>
                </ul>
                <details>
                    <summary>Click to reveal the correct answer</summary>
                    <p>The correct answer is C) Carbon dioxide</p>
                </details>
            </div>
        </div>

        <div class="question-container">
            <div class="question">
                <h2>Biology Question 3</h2>
                <p>What is the process by which organisms maintain a stable internal environment?</p>
                <ul>
                    <li>A) Homeostasis</li>
                    <li>B) Osmosis</li>
                    <li>C) Fermentation</li>
                    <li>D) Diffusion</li>
                </ul>
                <details>
                    <summary>Click to reveal the correct answer</summary>
                    <p>The correct answer is A) Homeostasis</p>
                </details>
            </div>
        </div>
    </div>
</body>
</html>
