# Simple Web Calculator

A basic, single-file web calculator built with HTML and vanilla JavaScript, capable of performing addition, subtraction, multiplication, and division. This project adheres to a minimalist approach, providing essential calculator functionality without external libraries.

## How to Use

1.  **Open in Browser:** Simply open the `index.html` file in your web browser.
2.  **Input Numbers:** Use the number buttons (0-9) to input digits.
3.  **Perform Operations:** Click an operator button (+, -, *, /) after entering the first number. Then, enter the second number.
4.  **Get Result:** Click the `=` button to display the result of the operation.
5.  **Chain Operations:** You can continue performing operations on the result (e.g., `5 + 3 = 8 + 2 = 10`).
6.  **Decimal Numbers:** Use the `.` button for decimal points.
7.  **Clear Display:** Click the `C` button to clear the current input and reset the calculator.
8.  **Division by Zero:** The calculator will display an alert and reset if you attempt to divide by zero.

## Code Explanation

This project is contained entirely within a single `index.html` file, demonstrating a self-contained web application.

*   **HTML Structure:** The HTML defines the calculator's user interface. It includes a `div` element acting as the display for numbers and results, and a grid of `<button>` elements for numbers, operators, a decimal point, clear function, and the equals sign.
*   **CSS Styling:** Embedded within a `<style>` tag in the `<head>`, the CSS provides the visual layout and styling. It uses CSS Grid to arrange the calculator buttons into a classic grid formation, along with basic styling for buttons, display, and overall appearance to make it user-friendly.
*   **JavaScript Logic:** Located at the end of the `<body>` in a `<script>` tag, the JavaScript is the core brain of the calculator.
    *   It maintains the calculator's state using variables like `currentInput` (what's currently shown), `firstOperand` (the first number in an operation), `operator` (the selected operation), and `waitingForSecondOperand` (a flag to manage input flow).
    *   Event listeners are attached to all buttons. When a button is clicked, a corresponding function (`inputDigit`, `inputDecimal`, `handleOperator`, `clearCalculator`, `operate`) is called.
    *   The `operate` function performs the actual arithmetic (+, -, \*, /) and includes basic error handling for division by zero.
    *   The `updateDisplay` function ensures the calculator's screen always reflects the current state.

## License

This project is licensed under the MIT License.