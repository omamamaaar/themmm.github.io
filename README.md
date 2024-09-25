<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>7 Questions Form</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f0f0f0;
            padding: 20px;
        }
        .container {
            max-width: 600px;
            margin: 0 auto;
            background-color: #fff;
            padding: 20px;
            border-radius: 8px;
            box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
        }
        h1 {
            text-align: center;
        }
        label {
            font-weight: bold;
            margin-top: 10px;
            display: block;
        }
        input[type="text"] {
            width: 100%;
            padding: 8px;
            margin-top: 5px;
            margin-bottom: 15px;
            border-radius: 4px;
            border: 1px solid #ccc;
        }
        button {
            display: block;
            width: 100%;
            padding: 10px;
            background-color: #007bff;
            color: white;
            border: none;
            border-radius: 4px;
            cursor: pointer;
        }
        button:hover {
            background-color: #0056b3;
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>Answer These 7 Questions</h1>
        <form id="questionsForm">
            <label for="q1">1. What is your name?</label>
            <input type="text" id="q1" name="q1">

            <label for="q2">2. What is your favorite hobby?</label>
            <input type="text" id="q2" name="q2">

            <label for="q3">3. Where do you live?</label>
            <input type="text" id="q3" name="q3">

            <label for="q4">4. What inspires you?</label>
            <input type="text" id="q4" name="q4">

            <label for="q5">5. What is your biggest challenge?</label>
            <input type="text" id="q5" name="q5">

            <label for="q6">6. What are your goals?</label>
            <input type="text" id="q6" name="q6">

            <label for="q7">7. What makes you happy?</label>
            <input type="text" id="q7" name="q7">

            <button type="button" onclick="nextPage()">Next</button>
        </form>
    </div>

    <script>
        function nextPage() {
            let form = document.getElementById('questionsForm');
            let answers = [];
            for (let i = 1; i <= 7; i++) {
                let answer = document.getElementById('q' + i).value;
                answers.push(answer);
            }

            console.log('Answers:', answers);
            // Here, you can add code to submit the data or move to the next step/page.
            alert('Your answers have been recorded!');

            // Redirect to a new page if needed
            // window.location.href = 'nextPage.html';
        }
    </script>
</body>
</html>
