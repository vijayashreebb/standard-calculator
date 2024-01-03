# Design of a Standard Calculator

## AIM:

To design a web application for a standard calculator.

## DESIGN STEPS:

### Step 1:
create a basic structure of your HTML file.

### Step 2:
style your calculator using CSS.


### Step 3:

add functionality to your calculator using javascript.


### Step 4:
inside you add buttons for numbers(0-9) operators (+,-,*,/).clear(c) and equal(=).

### Step 5:
improve CSS styling.

### Step 6:

Validate the HTML and CSS code.

### Step 6:

Publish the website in the given URL.

## PROGRAM :
<!DOCTYPE html>

<html lang="en">
<head>
<meta charset="UTF-8">
<title>Standard Calculator</title>
<style>
/* Basic styling for the calculator */
body {
font-family: Arial, sans-serif;
background-color: #f4f4f4;
}
.calculator {
width: 300px;
margin: 50px auto;
background-color: #fff;
border-radius: 5px;
box-shadow: 0 0 10px rgba(0,0,0,0.2);
padding: 20px;
}
input[type="text"] {
width: calc(100% - 10px);
margin-bottom: 10px;
padding: 10px;
font-size: 20px;
}
input[type="button"] {
width: 45px;
height: 45px;
margin: 5px;
font-size: 18px;
}
</style>
</head>
<body>
<div class="calculator">
<input type="text" id="display" disabled><br>
<input type="button" value="7" onclick="appendToDisplay('7')">
<input type="button" value="8" onclick="appendToDisplay('8')">
<input type="button" value="9" onclick="appendToDisplay('9')">
<input type="button" value="/" onclick="appendToDisplay('/')"><br>
<input type="button" value="4" onclick="appendToDisplay('4')">
<input type="button" value="5" onclick="appendToDisplay('5')">
<input type="button" value="6" onclick="appendToDisplay('6')">
<input type="button" value="*" onclick="appendToDisplay('*')"><br>
<input type="button" value="1" onclick="appendToDisplay('1')">
<input type="button" value="2" onclick="appendToDisplay('2')">
<input type="button" value="3" onclick="appendToDisplay('3')">
<input type="button" value="-" onclick="appendToDisplay('-')"><br>
<input type="button" value="0" onclick="appendToDisplay('0')">
<input type="button" value="." onclick="appendToDisplay('.')">
<input type="button" value="=" onclick="calculate()">
<input type="button" value="+" onclick="appendToDisplay('+')"><br>
<input type="button" value="C" onclick="clearDisplay()">
<input type="button" value="C" onclick="clearDisplay()">
</div>
<script>
function appendToDisplay(value) {
document.getElementById('display').value += value;
}
function calculate() {
const displayValue = document.getElementById('display').value;
if (displayValue) {
try {
const result = eval(displayValue);
document.getElementById('display').value = result;
} catch (error) {
document.getElementById('display').value = 'Error';
}
}
}
function clearDisplay() {
document.getElementById('display').value = '';
}
</script>
</body>
</html>


## OUTPUT:
![image](https://github.com/vijayashreebb/standard-calculator/assets/153714979/75294ec4-3ed7-4d73-ab11-d5939eb1dc04)

## Result:
Thus the program executed.
