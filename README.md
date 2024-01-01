# NAME    :KARTHICKKUMAR.R

# ROLL NO :23012023

## Experiment 03 Implementation of Half subtractor and Full subtractor circuit

## AIM:

To design a half subtractor and full subtractor circuit and verify its truth table in Quartus using Verilog programming.

## Equipments Required:

Hardware – PCs, Cyclone II , USB flasher
Software – Quartus prime

 ## Theory

 Subtractor circuits take two binary numbers as input and subtract one binary number input from the other binary number input. Similar to adders, it gives out two outputs, difference and borrow (carry-in the case 
 of Adder). There are two types of subtractors.

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

The combinational circuit of a full subtractor executes the operation of subtraction on three binary
bits generating outputs for the difference D and borrow B-out. Exactly like the binary adder circuit,
the full subtractor can also be imagined as two half subtractors connected together as shown
below. A full subtractor can be realized using two half subtractors. It will take two half-subtractors
and one OR gate. The logic circuit diagram of the full subtractor using two half subtractors A Half
subtractor is a combination circuit with two inputs and two outputs that are different and borrow. It
produces the difference between the two binary bits at the input and also produces an output
(Borrow) to indicate if a 1 has been borrowed.


## Program:

![WO4 P](https://github.com/vasanthkumarch/Experiment--03-Half-Subtractor-and-Full-subtractor/assets/150005103/8d300b47-e57b-41ec-a95d-55b36de7c49d)

##  RTL realization

HALF SUBTRACTOR

![WO4 LH](https://github.com/vasanthkumarch/Experiment--03-Half-Subtractor-and-Full-subtractor/assets/150005103/145b21d6-e93d-48df-a479-e52c04a77e73)

FULL SUBTRACTOR

![WO4LF](https://github.com/vasanthkumarch/Experiment--03-Half-Subtractor-and-Full-subtractor/assets/150005103/b430130b-96ce-4bda-a5a2-7fc31a08c360)

## Truthtable

HALF SUBTRACTOR

![WO4TTH](https://github.com/vasanthkumarch/Experiment--03-Half-Subtractor-and-Full-subtractor/assets/150005103/8e70fd8b-7473-48fd-b450-07f639307078)

FULL SUBTRACTOR

![WO4 TTF](https://github.com/vasanthkumarch/Experiment--03-Half-Subtractor-and-Full-subtractor/assets/150005103/6de3b7c9-cdb7-45ea-88fa-31e47fd6ea01)

## Timing diagram 

HALF SUBTRACTOR

![WO4 TDH](https://github.com/vasanthkumarch/Experiment--03-Half-Subtractor-and-Full-subtractor/assets/150005103/e97c2bdf-5421-4fad-8cfb-f6439aae4647)

FULL SUBTRACTOR

![WO4 TDF](https://github.com/vasanthkumarch/Experiment--03-Half-Subtractor-and-Full-subtractor/assets/150005103/940c59e1-420b-41aa-9986-4ed662357a1e)

## Result:
Thus the half subtractor and full subtractor circuits are designed and the truth tables is verified using quartus software.
