# full_suber

Implementation-of-Full-subtractor-circuit

AIM:

To design a Full Subtractor circuit and VERIFY IN Quartus using Verilog programming.

Equipments Required:

     Hardware – PCs, Cyclone II , USB flasher

Software – Quartus prime

 Full Subtractor

A full subtractor is a combinational circuit that performs subtraction involving three bits, namely minuend, subtrahend, and borrow-in .
It accepts three inputs: minuend, subtrahend and a borrow bit and it produces two outputs: difference and borrow.

Diff = A ⊕ B ⊕ Bin

Borrow out = A'Bin + A'B + BBin

Program:

```

module full_subtractor (
    input  wire a, b, bin,       // Inputs
    output wire diff, borrow     // Outputs
);

    // Logic equations
    assign diff   = a ^ b ^ bin;                  // Difference
    assign borrow = (~a & b) | (~(a ^ b) & bin);  // Borrow logic

endmodule

```

RTL Schematic:

[EX 04 sub.pdf](https://github.com/user-attachments/files/24141315/EX.04.sub.pdf)

Output Timing Waveform:

[unknown.bmp](https://github.com/user-attachments/files/24141316/unknown.bmp)

NAME: TAMIZHAN.B

REF NO: 25018064

Result:

Thus the Full Adder circuits are designed is verified using Quartus software.

