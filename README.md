<div style="font-family: Arial, sans-serif; max-width: 800px; margin: 0 auto; padding: 20px; border: 1px solid #ccc;">

    <h1 style="border-bottom: 2px solid #eee; padding-bottom: 10px;">Simple Calculator (Calcolatrice Semplice)</h1>

    <p>This is a single-file, web-based calculator application built using <strong>HTML, CSS, and vanilla JavaScript</strong>.</p>
    <p>It simulates a basic arithmetic calculator with functionality for addition, subtraction, multiplication, and division, and includes a history log.</p>

    <hr style="margin-top: 20px; margin-bottom: 20px;">

    <h2 style="color: #333;">Features</h2>

    <ul style="list-style-type: disc; padding-left: 20px;">
        <li><strong>Basic Arithmetic:</strong> Supports addition ($+$), subtraction ($-$), multiplication ($\times$), and division ($\div$).</li>
        <li><strong>Decimal Support:</strong> Allows for floating-point calculations.</li>
        <li><strong>Operation Chaining:</strong> You can string multiple operations together (e.g., $10 + 5 \times 2 - 3$).</li>
        <li><strong>History Log (Cronologia):</strong> Stores a record of all completed calculations until the history is viewed.</li>
        <li><strong>Clear Function (AC):</strong> Resets the display and the current operation.</li>
        <li><strong>Responsive Design:</strong> Styled to be functional and aesthetically pleasing on different screen sizes.</li>
    </ul>

    <hr style="margin-top: 20px; margin-bottom: 20px;">

    <h2 style="color: #333;">Usage</h2>

    <p>The calculator is contained entirely within the <code>calculator evo.html</code> file.</p>

    <ol style="padding-left: 20px;">
        <li><strong>Download:</strong> Save the <code>calculator evo.html</code> file to your local machine.</li>
        <li><strong>Open:</strong> Double-click the file or open it with any modern web browser (Chrome, Firefox, Edge, Safari, etc.).</li>
        <li><strong>Calculate:</strong> Click the numbered buttons to input digits. Use the operator buttons ($\div, \times, -, +$) to perform operations.</li>
        <li><strong>View History:</strong> Click the <strong>"Cronologia"</strong> button to see a list of all calculations performed since the last time the history was viewed.</li>
    </ol>

    <hr style="margin-top: 20px; margin-bottom: 20px;">

    <h2 style="color: #333;">Technical Details</h2>

    <p>The application is structured using a simple state machine approach in JavaScript:</p>
    <ul style="list-style-type: square; padding-left: 20px;">
        <li><strong><code>display.textContent</code></strong>: Stores the current visible input/result.</li>
        <li><strong><code>firstOperand</code></strong>: Stores the first number of the current operation.</li>
        <li><strong><code>currentOperator</code></strong>: Stores the operator ($+, -, \times, \div$) pending execution.</li>
        <li><strong><code>waitingForSecondOperand</code></strong>: A boolean flag to manage input state after an operator has been pressed.</li>
        <li><strong><code>chrono</code></strong>: An array used to store the history of calculations.</li>
    </ul>
    <p>The core logic is handled by functions like <code>inputDigit</code>, <code>handleOperator</code>, <code>calculate</code>, and <code>handleEquals</code>.</p>

</div>
