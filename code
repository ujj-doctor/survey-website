<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Simple Survey</title>
    <style>
        body {
            margin: 0;
            font-family: Arial, sans-serif;
            display: grid;
            place-items: center;
            height: 100vh;
            background: #f0f0f0;
        }

        #surveyContainer {
            background: white;
            padding: 20px;
            border-radius: 8px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
            max-width: 500px;
            width: 100%;
            animation: fadeIn 0.5s ease-in-out;
        }

        h2 {
            text-align: center;
            margin-bottom: 20px;
        }

        .question {
            margin-bottom: 15px;
        }

        label {
            display: block;
            margin-bottom: 5px;
        }

        input[type="text"], input[type="email"], textarea {
            width: 100%;
            padding: 10px;
            border: 1px solid #ddd;
            border-radius: 4px;
            box-sizing: border-box;
        }

        textarea {
            resize: vertical;
        }

        button {
            width: 100%;
            padding: 10px;
            background: #14143a;
            color: rgb(236, 229, 229);
            border: none;
            border-radius: 4px;
            cursor:pointer;
            margin-top: 20px;
            transition: background 0.3s ease;
        }

        button:hover {
            background: #3700b3;
        }

        #thankYou {
            display: none;
            text-align: center;
            animation: fadeIn 0.5s ease-in-out;
        }

        @media (max-width: 600px) {
            #surveyContainer {
                padding: 15px;
            }
        }

        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(20px); }
            to { opacity: 1; transform: translateY(0); }
        }
    </style>
</head>
<body>

<div id="surveyContainer">
    <h2>Customer Feedback Survey</h2>

    <div class="question">
        <label for="name">Your Name:</label>
        <input type="text" id="name" required>
    </div>

    <div class="question">
        <label for="email">Your Email:</label>
        <input type="email" id="email" required>
    </div>

    <div class="question">
        <label for="feedback">Your Feedback:</label>
        <textarea id="feedback" rows="4" required></textarea>
    </div>

    <button onclick="submitSurvey()">Submit</button>
</div>

<div id="thankYou">
    <h3>Thank you for your feedback!</h3>
    <button onclick="submitAnother()">Submit Another Response</button>
</div>

<script>
    function submitSurvey() {
        document.getElementById('surveyContainer').style.display = 'none';
        document.getElementById('thankYou').style.display = 'block';
    }

    function submitAnother() {
        document.getElementById('surveyContainer').style.display = 'block';
        document.getElementById('thankYou').style.display = 'none';
        document.getElementById('name').value = '';
        document.getElementById('email').value = '';
        document.getElementById('feedback').value = '';
    }
</script>

</body>
</html>

