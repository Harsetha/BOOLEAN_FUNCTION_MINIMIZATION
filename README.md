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

/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

module Boolean_min(a,b,c,d,w,x,y,z,f1,f2);
input a,b,c,d,w,x,y,z;
output f1,f2;
wire adash,bdash,cdash,ddash,ydash,p,q,r,s,t,u;
not(adash,a);
not(bdash,b);
not(cdash,c);
not(ddash,d);
and(p,bdash,ddash);
and(q,adash,b,d);
and(r,a,b,cdash);
or(f1,p,q,r);
not(ydash,y);
and(s,ydash,z);
and(t,x,y);
and(u,w,y);
or(f2,s,t,u);
endmodule


Developed by:HARSETHA J
RegisterNumber:212223220032



**RTL realization**
![316316875-735f5bd3-cf3b-4c34-b2fb-f50eafa8de7d](https://github.com/Harsetha/BOOLEAN_FUNCTION_MINIMIZATION/assets/149985878/24685bcd-0d4f-48a7-830a-19f28126bd44)


**Output:**
![316316898-88ef005e-96dc-4f77-9439-1a922ea69501](https://github.com/Harsetha/BOOLEAN_FUNCTION_MINIMIZATION/assets/149985878/22f104b0-6a3c-435b-a540-f301ae73c17a)



**RTL**
![316316854-a881cd5b-0761-4f38-b95c-51f1e0358077](https://github.com/Harsetha/BOOLEAN_FUNCTION_MINIMIZATION/assets/149985878/84629c21-d654-4bab-b133-20b5d6e57fa9)


**Timing Diagram**

## Result:

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

