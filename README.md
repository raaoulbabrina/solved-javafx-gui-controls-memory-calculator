Download Link: https://assignmentchef.com/product/solved-javafx-gui-controls-memory-calculator
<br>
5/5 - (2 votes)

 This is the last homework assignment in this course, and it is meant to show you how a small but complete GUI application is structured. We will make our GUI actually control our memory calculator.

To do this, you will need to create an instance of MemoryCalc in the CalcGUI and write event Handlers to pass information back and forth between the calculator and the GUI. There are many possible ways to achieve this, but the easiest is probably to develop four different event

Handlers:DigitHandler – This event Handler is added to the 0-9 and . (dot) keys. If the equals button was just pressed, this event Handler will overwrite the total shown in the text field with the value of the key (its label) that was just pressed. If the equals button was not just pressed, this event Handler will append the current key’s label onto the end of the string shown in the text field.

OperatorHandler – This event Handler is added to the +, -, *, and / keys. It sets the value of a class field to the operator that the user has chosen.

ClearHandler – This event Handler is added to the C key. It calls the calculator’s clear method and sets the value of the text field back to 0.0.

EqualsHandler – This event Handler is added to the = key. It reads the current value from the text field, converts it to a double, and calls the appropriate calculator method based on the current operator, passing in the double value. The calculator will compute the answer, and then this event Handler will update the value in the text field to the calculator’s current total.

That is all that required for the homework assignment, however I also encourage you to play around with the different types of calculators we have written in this course, perhaps after this course ends. For instance, you could add functionality for geometric operations like sine and cosine. Or you could create a Super Calculator that has different views for scalar, vector, and matrix calculations.

Whatever you come up with, I suggest you clean it up and document it. Potential employers always look favorably on being able to review code you have written and ask you questions about it. Hints: You can use the ActionEvent’s getSource() method to get a reference to the button that was pressed, and you can use Button’s getText() method to find out the label of that button.

When the EqualsHandler is converting the text shown in the text field into a double value in order to pass it to the calculator, be careful to handle the case where the text field contains an invalid value, such as 6..72. In this case you should catch the exception, display an error message to the user, and abort the call to the calculator (just restore the current total to the text field).

The user should only be able to enter numbers between when an operator has been selected and when the equals button has been pushed. The DigitHandler should ignore any button presses when the GUI is not in this state. Sample output: Please view the video homework.swf to see what the output of this topic’s assignment should be.

You will be graded according to the following rubric: · Something happens when the user clicks on any of the keys of the calculator JavaFX GUI:2 points · The user cannot enter a value without first choosing an operator:2 points · The user is able to enter numbers correctly (i.e. the previous total is overwritten when the user starts a new number, and new digits are appended to the new number):2 points · When the equals button is pressed, the appropriate calculator method is called based on the operator the user has selected:2 points · When the equals button is pressed, the appropriate operand passed to the calculator method as an argument:2 points · When the equals button is pressed, the value in the text field is updated to the new total:2 points · The clear button calls the calculator’s clear method and updates the text field to 0.0: 2 points · If the user enters an invalid value, an error message is displayed: 2 points · Your program compiles: 2 points ·

Your program runs:1 point · You follow standard coding conventions (e.g. variable names, indentation, comments, etc.):1 point · Note: If your program does not compile, you will receive a score of 0 on the entire assignment · Note: If you program compiles but does not run, you will receive a score of 0 on the entire assignment ·