# saseka-my-calculator-project
1.Project summary
HTML


<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Percentage Calculator</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <div class="calculator">
        <h2>Percentage Calculator</h2>
        <input type="number" id="number" placeholder="Enter the number">
        <input type="number" id="percentage" placeholder="Enter the percentage">
        <button onclick="calculatePercentage()">Calculate</button>
        <div id="result"></div>
    </div>

    <script src="script.js"></script>
</body>
</html>
CSS (styles.css)
css

body {
    font-family: Arial, sans-serif;
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100vh;
    margin: 0;
    background-color: #f4f4f4;
}

.calculator {
    background: white;
    padding: 20px;
    border-radius: 5px;
    box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
    text-align: center;
}

input {
    margin: 10px 0;
    padding: 10px;
    width: 80%;
    border: 1px solid #ddd;
    border-radius: 5px;
}

button {
    padding: 10px 20px;
    background-color: #007BFF;
    color: white;
    border: none;
    border-radius: 5px;
    cursor: pointer;
}

button:hover {
    background-color: #0056b3;
}

#result {
    margin-top: 20px;
    font-size: 18px;
    color: #333;
}
JavaScript (script.js)
javascript

function calculatePercentage() {
    const number = parseFloat(document.getElementById('number').value);
    const percentage = parseFloat(document.getElementById('percentage').value);
    if (!isNaN(number) && !isNaN(percentage)) {
        const result = (number * percentage) / 100;
        document.getElementById('result').textContent = `Result: ${result}`;
    } else {
        document.getElementById('result').textContent = 'Please enter valid numbers';
    }
}
Explanation
HTML: Sets up the basic structure with two input fields for the number and percentage, a button to calculate, and a div to display the result.
CSS: Styles the layout to center the calculator, with a clean and simple design.
JavaScript: Defines the function calculatePercentage to compute the percentage and display the result or an error message.


![ERD_diagram (1)](https://github.com/Saseka/saseka-my-calculator-project/assets/170074891/7af6b725-2c8f-40d7-8706-08cad254cfc8)








