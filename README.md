# BOOLEAN_FUNCTION_MINIMIZATION

*AIM:*

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

*Equipment Required:*

Hardware – PCs, Cyclone II , USB flasher

*Software – Quartus prime*

*Theory*
Boolean Algebra is a branch of algebra that deals with boolean values—true and false. It is fundamental to digital logic design and computer science, providing a mathematical framework for describing logical operations and expressions

*Boolean Expression*
(i)F1
![image](https://github.com/user-attachments/assets/3105f968-b821-455a-8377-9451ac013f51)

(ii)F2
![image](https://github.com/user-attachments/assets/0c1331bf-4459-489d-87c0-63c9dcac3717)

*Truth Table*


(i)F1

![image](https://github.com/user-attachments/assets/8a092861-2260-43b0-9bbd-173838521f3c)

(ii)F2

![image](https://github.com/user-attachments/assets/4528e7eb-7ef6-45cf-be4a-a6ea477b41db)

*Procedure*

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


*Program:*

 Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by: RAGA SUSANTH
RegisterNumber: 212224230217

        i)F1
        module funct1(a,b,c,d,f1);
        input a,b,c,d;
        output f1;
        assign f1=((~b & ~d)|(~a & b & d)|(a & b & ~c));
        endmodule

      ii)F2
      module funct2(w,x,y,z,f2);
      input w,x,y,z;
      output f2;
      assign f2=((~y & z)|( w & y )|(x & y));
      endmodule



*RTL realization*


(i)F1


![image](https://github.com/user-attachments/assets/3275b325-b554-447e-94de-dda82c65d105)

(ii)F2

![image](https://github.com/user-attachments/assets/1110d486-74e4-4de7-bef4-67e66d1a0820)


*Timing Diagram*


(i)F1

![image](https://github.com/user-attachments/assets/5c1c8a45-cd11-4e88-bfe6-9d04a91855e9)

(ii)F2

![image](https://github.com/user-attachments/assets/34f8c7fe-5521-4615-9cb4-faeae70370ed)


*Result:*

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.
