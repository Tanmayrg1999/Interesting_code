# Interesting_code
In this code I have declared and initialised 3 variables i.e. a=10 , b=20 , c=30 and just attached a conditioanal operator with condition c>b>a which appeals to be mathematically correct ,but instead it is not executed  instead the control is handeled by the else condition. 
The main reason for this behaviour is that **c>b>a** is not equivalent to **c>b &amp;&amp; b>a**.
Instead the equation is reduced to **(c>b)>a** and **c>b** holds true and true is a logical operator which is equivalent to 1 in binary or decimal number system.
So according to the BODMAS Rule Brackets are resolved first hence c>b i.e. 30>20 holds true and returns the value 1 and therefor the corresponding bracket contains the value and thus the equation **30>20>10** reduces to **1>20** which is false hence the if condition is not true hence the else block is executed. Hence the output is false in this condition.
