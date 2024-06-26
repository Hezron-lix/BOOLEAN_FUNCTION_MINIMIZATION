# BOOLEAN_FUNCTION_MINIMIZATION

**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher

**Software – Quartus prime**

**Theory**

**Logic Diagram**

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

module booleanfunction_top(a,b,c,d,w,x,y,z,f1,f2);
input a,b,c,d,w,x,y,z;
output f1,f2;
wire adash,bdash,cdash,ddash,ydash,p,q,r,s,t,u;
not(adash,a);
not(bdash,b);
not(cdash,c);
not(ddash,d);
not(ydash,y);
and(p,bdash,ddash);
and(q,adash,b,d);
and(r,a,b,cdash);
or(f1,p,q,r);
//type code for f2 as like f1
endmodule

/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming.

Developed by: Hezron Belix P

RegisterNumber: 212223230078
*/

**Output:**

![313538446-9ea152f7-b7da-46ba-b9c3-086243fcf7e3](https://github.com/Hezron-lix/BOOLEAN_FUNCTION_MINIMIZATION/assets/139331337/c1ab959b-f2d2-4ae1-8ff2-0c82e3453e3a)

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

