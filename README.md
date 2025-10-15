# Simple Calculator (Calcolatrice Semplice) 🧮

This is a single-file, web-based calculator application built using **HTML, CSS, and vanilla JavaScript**.

It simulates a basic arithmetic calculator with functionality for addition, subtraction, multiplication, and division, and includes a history log.

---

## Features ✨

* **Basic Arithmetic:** Supports addition ($+$), subtraction ($-$), multiplication ($\times$), and division ($\div$).
* **Decimal Support:** Allows for floating-point calculations.
* **Operation Chaining:** You can string multiple operations together (e.g., $10 + 5 \times 2 - 3$).
* **History Log (Cronologia):** Stores a record of all completed calculations until the history is viewed.
* **Clear Function (AC):** Resets the display and the current operation.
* **Responsive Design:** Styled to be functional and aesthetically pleasing on different screen sizes.

---

## Usage 💻

The calculator is contained entirely within the `simple calculator.html` file.

1.  **Download:** Save the `simple calculator.html` file to your local machine.
2.  **Open:** Double-click the file or open it with any modern web browser (Chrome, Firefox, Edge, Safari, etc.).
3.  **Calculate:** Click the numbered buttons to input digits. Use the operator buttons ($\div, \times, -, +$) to perform operations.
4.  **View History:** Click the **"Cronologia"** button to see a list of all calculations performed since the last time the history was viewed.

---

## Technical Details ⚙️

The application is structured using a simple state machine approach in JavaScript:

* `display.textContent`: Stores the current visible input/result.
* `firstOperand`: Stores the first number of the current operation.
* `currentOperator`: Stores the operator ($+, -, \times, \div$) pending execution.
* `waitingForSecondOperand`: A boolean flag to manage input state after an operator has been pressed.
* `chrono`: An array used to store the history of calculations.

The core logic is handled by functions like `inputDigit`, `handleOperator`, `calculate`, and `handleEquals`.
