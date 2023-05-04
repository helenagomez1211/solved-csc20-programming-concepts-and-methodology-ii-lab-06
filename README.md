Download Link: https://assignmentchef.com/product/solved-csc20-programming-concepts-and-methodology-ii-lab-06
<br>
<strong>Objective: </strong>

The objective of this lab is to get you some experience in processing strings character by character and in implementing stacks and queues in a class package.




<strong>The programming assignment</strong>:

In your lab05, replace instructor’s Tokenizer class and MyStackQueue package with your own.

<strong>Requirements</strong>:




<ol>

 <li>You must use a linked list to implement your queue.</li>

 <li>You must use an array to implement your stack.</li>

 <li>You must use the following frame work to implement your tokenizer.</li>

</ol>




class Tokenizer { private char [] Buf;

private int cur;




Tokenizer(String infixExpression) { Buf = infixExpression.toCharArray(); cur = 0;

}




boolean moreTokens() {

Skip blanks.

return cur&lt;Buf.length;

}




Token nextToken() { 1. Skip blanks.




<ol start="2">

 <li>if (cur&gt;=Buf.length) return null;</li>

</ol>




<ol start="3">

 <li>If the next character is a digit, keep reading until a non-digit is read. Convert the string of digits into an integer.</li>

</ol>




String Digits = new String(Buf, start, len);

int num = Integer.valueOf(Digits).intValue();




Use num to create and return an operand.




<ol start="4">

 <li>Otherwise, use the next character to create and return an operator.</li>

</ol>

}

}