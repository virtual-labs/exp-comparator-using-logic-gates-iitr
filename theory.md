### Introduction

A magnitude digital comparator is a combinational circuit that compares two digital or binary numbers in order to find out whether one binary number is equal, less than or greater than the other binary number. We logically design a circuit for which we will have two inputs one for A and other for B and have three output terminals, one for A > B condition, one for A = B condition and one for A < B condition.<br><br>
                    	
<center><img src="images/aa.png"  width="300" height="150"> 

<b>Figure-1: Block Diagram of Comparator </b></p> </center><br>
      
  

### 1) 1-Bit Magnitude Comparator : 
A comparator used to compare two bits is called a single bit comparator. It consists of two inputs each for two single bit numbers and three outputs to generate less than, equal to and greater than between two binary numbers. The truth table for a 1-bit comparator is given below :<br>
					 	                    
<center><img src="images/ab.png"  width="300" height="200"><br> <b>Figure-2: Truth Table of 1-Bit Comparator</b> <br></center>
      

From the above truth table logical expressions for each output can be expressed as follows:<br>
A > B : AB'<br>
A < B : A'B<br>
A = B : A'B' + AB<br><br>
By using these Boolean expressions, we can implement a logic circuit for this comparator as given below :<br>
              	
<center><img src="images/ac.png"  width="500" height="250"> <br><b>Figure-3: Logic Circuit of 1-Bit Comparator</b><br></center>
      
  

### 2) 2-Bit Magnitude Comparator :
A comparator used to compare two binary numbers each of two bits is called a 2-bit magnitude comparator. It consists of four inputs and three outputs to generate less than, equal to and greater than between two binary numbers.<br>

The truth table for a 2-bit comparator is given below:<br>
<center><img src="images/Digitallogic4.png"  width="500" height="400"> <br><b>Figure-4: Truth Table of 2-Bit Comparator</b></center> <br>
      

From the above truth table logical expressions for each output can be expressed as follows:<br>
A > B : A<sub>1</sub>B<sub>1</sub>’ + A<sub>0</sub>B<sub>1</sub>’B<sub>0</sub>’ + A<sub>1</sub>A<sub>0</sub>B<sub>0</sub>’<br>
A = B : A<sub>1</sub>’A<sub>0</sub>’B<sub>1</sub>’B<sub>0</sub>’ + A<sub>1</sub>’A<sub>0</sub>B<sub>1</sub>’B<sub>0</sub> + A<sub>1</sub>A<sub>0</sub>B<sub>1</sub>B<sub>0</sub> + A<sub>1</sub>A<sub>0</sub>’B<sub>1</sub>B<sub>0</sub>’<br>
   &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;: A<sub>1</sub>’B<sub>1</sub>’ (A<sub>0</sub>’B<sub>0</sub>’ + A<sub>0</sub>B<sub>0</sub>) + A<sub>1</sub>B<sub>1</sub> (A<sub>0</sub>B<sub>0</sub> + A<sub>0</sub>’B<sub>0</sub>’)<br>
  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;: (A<sub>0</sub>B<sub>0</sub> + A<sub>0</sub>’B<sub>0</sub>’) (A<sub>1</sub>B<sub>1</sub> + A<sub>1</sub>’B<sub>1</sub>’)<br>
   &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;: (A<sub>0</sub> Ex-Nor B<sub>0</sub>) (A<sub>1</sub> Ex-Nor B<sub>1</sub>)<br>
A < B : A<sub>1</sub>’B<sub>1</sub> + A<sub>0</sub>’B<sub>1</sub>B<sub>0</sub> + A<sub>1</sub>’A0’B0<br><br>
By using these Boolean expressions, we can implement a logic circuit for this comparator as given below :<br><br>
              	
<center><img src="images/ae.png"  width="500" height="350"><br> <b>Figure-5: Logic Circuit of 2-Bit Comparator</b></center><br>
      
  
### Applications of Comparators : 
1. Comparators are used in central processing units (CPUs) and microcontrollers (MCUs).<br>
2. These are used in control applications in which the binary numbers representing physical variables such as temperature, position, etc. are compared with a reference value.<br>
3. Comparators are also used as process controllers and for Servo motor control.<br>
4. Used in password verification and biometric applications.
      



