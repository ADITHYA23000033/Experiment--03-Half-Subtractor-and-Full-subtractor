# Experiment--03-Half-Subtractor-and-Full-subtractor
## Implementation-of-Half-subtractor-and-Full-subtractor-circuit
## AIM:
To design a half subtractor and full subtractor circuit and verify its truth table in Quartus using Verilog programming.

## Equipments Required:
## Hardware – PCs, Cyclone II , USB flasher
## Software – Quartus prime
## Theory
Subtractor circuits take two binary numbers as input and subtract one binary number input from the other binary number input. Similar to adders, it gives out two outputs, difference and borrow (carry-in the case of Adder). There are two types of subtractors.

## Half Subtractor Full Subtractor
## Half Subtractor
The half-subtractor is a combinational circuit which is used to perform subtraction of two bits. It has two inputs, X (minuend) and Y (subtrahend) and two outputs D (difference) and B (borrow). To perform x - y, we have to check the relative magnitudes of x and y. If x ;;, y, we have three possibilities: 0 - 0 = 0, 1 - 0 = 1, and 1 - I = 0. The result is called the difference bit. If x < y, we have 0 - I, and it is necessary to borrow a 1 from the next higher stage. The I borrowed from the next higher stage adds 2 to the minuend bit, just as in the decimal system a borrow adds 10 to a minuend digit. With the minuend equal to 2, the difference becomes 2 - I = 1. The half-subtractor needs two outputs. One output generates the difference and will be designated by the symbol D. The second output, designated B for borrow, generates the binary signal that informs the next stage that a I has been borrowed.
![half-subtractor9](https://user-images.githubusercontent.com/36288975/166112538-58c3bc7c-ee5d-4e6a-ac8d-8e8328efe27a.png)


Sum = X'Y+XY' = X ⊕ Y
Carry=X'Y

## Full Subtractor
A full subtractor is a combinational circuit that performs subtraction involving three bits, namely minuend, subtrahend, and borrow-in . It accepts three inputs: minuend, subtrahend and a borrow bit and it produces two outputs: difference and borrow. 
![full-subtractor6](https://user-images.githubusercontent.com/36288975/166112541-24c68359-3de8-4674-ae22-8272ffc385ed.png)


Diff = A ⊕ B ⊕ Bin B = A'Bin + A'B + BBin

## Procedure

STEP 1: Use module project name(input,output) to start the Verilog programmming.
STEP 2: Assign inputs and outputs using the word input and output respectively.
STEP 3: Use defined keywords like wire,assign and required logic gates to represent the boolean expression.
STEP 4: Use each output to represnt onre for differnce and the other for borrow.
STEP 5: End the verilog program using keyword endmodule. 


## Program:
/*
Program to design a half subtractor and full subtractor circuit and verify its truth table in quartus using Verilog programming.

Developed by: ADITHYA V

RegisterNumber: 23000033
*/

half subracter

![Exp4 hs code](https://github.com/ADITHYA23000033/Experiment--03-Half-Subtractor-and-Full-subtractor/assets/148514544/99c72620-d6aa-4f51-abcd-b0bd2d6e0aa5)

full subracter

![Exp4 fs code](https://github.com/ADITHYA23000033/Experiment--03-Half-Subtractor-and-Full-subtractor/assets/148514544/dc7a29bc-ee12-4d67-88d4-0fcc2e114993)

## Output:

## Truthtable

half subracter

![Exp4 truthtable hs](https://github.com/ADITHYA23000033/Experiment--03-Half-Subtractor-and-Full-subtractor/assets/148514544/8c2b1132-eabf-4e76-b78f-0c0c49e571fb)

full subracter

![Exp4 truthtable fs](https://github.com/ADITHYA23000033/Experiment--03-Half-Subtractor-and-Full-subtractor/assets/148514544/a8916692-adac-4715-b819-ff65a2aebe41)

##  RTL realization

half subracter

![Exp4 hs RTL diagram](https://github.com/ADITHYA23000033/Experiment--03-Half-Subtractor-and-Full-subtractor/assets/148514544/21ff9437-b1bc-4652-b873-f0e44d30b68f)

full subracter

![Exp4 fs RTL diagram](https://github.com/ADITHYA23000033/Experiment--03-Half-Subtractor-and-Full-subtractor/assets/148514544/52a60061-ff51-4cc5-93bd-cc2e4ac1e7c3)

## Timing diagram 

half subracter

![hs wave](https://github.com/ADITHYA23000033/Experiment--03-Half-Subtractor-and-Full-subtractor/assets/148514544/8122a67e-2e61-45fa-bb5c-7e8c1baf91e0)

full subracter

![fs wave](https://github.com/ADITHYA23000033/Experiment--03-Half-Subtractor-and-Full-subtractor/assets/148514544/8f7cad2b-20d6-4173-aed6-17a0f0115fdc)

## Result:
Thus the half subtractor and full subtractor circuits are designed and the truth tables is verified using quartus software.
