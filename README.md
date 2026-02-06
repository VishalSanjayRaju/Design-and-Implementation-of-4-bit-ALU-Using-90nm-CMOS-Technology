# Design-and-Implementation-of-4-bit-ALU-Using-90nm-CMOS-Technology

A 4-bit Arithmetic Logic Unit or also called as ALU is a digital circuit that performs a range of arithmetic and logical operations on 4-bit binary numbers. As one of the core components in processors, the ALU enables execution of basic calculations and decision-making tasks, serving as the "computational brain" within microprocessors, digital signal processors (DSPs), and embedded systems. By working with 4-bit data units, this ALU is suited for small-scale computing applications and educational purposes, providing a compact yet functional approach. The ALU consists of many blocks like adder, subtractor, magnitude comparator, shift register, 2’s complement, 1’s complement, divider, decoder and multiplier, 

The 4-bit ALU design typically includes two main categories that is, arithmetic operations for numerical calculations and logical operations for bitwise manipulations. This design enables efficient processing of data, allowing for basic computing and control logic functions that are essential in various digital systems. Implementing a 4-bit ALU also provides insights into the key principles of digital design, such as binary arithmetic, circuit simplification, and the integration of logical gates to achieve multifunctional capability. Its simplicity makes it a versatile tool in digital electronics, ideal for introductory learning as well as foundational experiments in more complex digital architectures.

This report presents the design and implementation of a 4-bit Arithmetic Logic Unit (ALU) using Cadence Virtuoso software, making use of the 90nm CMOS technology node. The 4-bit ALU serves as a fundamental component in digital processors, performing a range of essential arithmetic and logical operations on binary data. Designed with compactness and efficiency in mind, the ALU can execute basic functions such as addition, subtraction, magnitude comparison, shifting of data i.e. left shift and right shift, 2’s complement, 1’s complement, division, decoder block, and multiplication all critical for various computational tasks in microprocessors, digital signal processing units, and embedded systems. By using 90nm CMOS technology, the ALU achieves a balance between performance, area, and power consumption, which is crucial in modern, resource-constrained digital circuits.

The design process in Virtuoso involved rigorous steps from schematic design and simulation to layout generation, following industry-standard practices to ensure accuracy and manufacturability. The 90nm technology node was chosen for its ability to offer good speed and moderate power consumption, making it suitable for low-power applications. Extensive testing and analysis were performed to verify the ALU’s performance and reliability, with parameters such as delay, power consumption, and static noise margin carefully evaluated. 

METHODOLOGY

In this project, the methodology for designing the 4-bit adder, 4-bit subtractor, 4-bit magnitude comparator, 3:8 decoder and 4-bit 1’s complement was based on 90nm CMOS technology using Cadence Virtuoso. The first step involved creating the schematics for each of the components. For the 4-bit adder and subtractor, full adders and subtractors were designed using CMOS logic gates, ensuring that both operations could handle 4-bit inputs and produce accurate sum and difference outputs. The 4-bit magnitude comparator was designed to compare two 4-bit inputs and generate the corresponding output based on equality, greater than, or less than conditions. The 3:8 bit decoder will decode the input 3-bit and give the 8-bit output. The 4-bit 1’s complement will invert the input 2 4-bit and give 2 4-bit as output. After the schematic design, the next step was to create the corresponding test benches for all five blocks. These test benches were constructed to validate the functionality of the blocks under various input conditions, simulating both normal and edge cases.

Following the schematic and test bench creation, the waveform analysis was performed using Cadence Virtuoso’s simulation tools. The simulation allowed for observing the behaviour of the designed circuits under different input combinations and ensured that the outputs met the expected results. By analysing the waveforms, any discrepancies in the operation, such as incorrect outputs or timing issues, could be identified and rectified. The simulation results confirmed the correct functionality of the 4-bit adder, subtractor, magnitude comparator, 1’s complement and decoder. This process of schematic design, test bench creation, and waveform analysis ensured the reliability and correctness of the individual blocks, laying a solid foundation for their integration into a larger ALU design.

 <img width="906" height="423" alt="image" src="https://github.com/user-attachments/assets/4a52bc15-5ba1-4a4f-bfe6-65415ca5a108" />

Schematic of the Full adder

 <img width="874" height="410" alt="image" src="https://github.com/user-attachments/assets/ea73f35e-09f5-4eba-8269-43126391b608" />

Layout of the Full adder

The image above shows the schematic diagram and layout of a 4-bit full adder implemented using 90nm CMOS technology. This full adder takes three inputs: A, B, and Carry-in (Cin), and produces two outputs: Sum and Carry-out (Cout). The design utilizes basic CMOS logic gates, including NAND, NOR, and XOR gates, to achieve the desired arithmetic functionality. The full adder's role is to perform the addition of two binary bits along with a carry-in bit, generating a sum and a carry-out bit. The schematic demonstrates the integration of these logic gates, ensuring that the full adder functions correctly within the larger 4-bit adder block. The use of CMOS technology ensures low power consumption and high-speed performance, crucial for efficient digital circuit design.

<img width="886" height="779" alt="image" src="https://github.com/user-attachments/assets/d6e76140-3fae-4147-bc95-b54262a9ae54" />

Schematic of the subtractor

 <img width="465" height="536" alt="image" src="https://github.com/user-attachments/assets/031a60e6-ab27-48f2-bd0a-4bf81cca77b3" />

layout of the subtractor

The image above shows the schematic diagram and layout design of the 4-bit subtractor designed using 90nm CMOS technology. This subtractor is responsible for performing the subtraction operation on two 4-bit binary numbers. It takes two inputs: A and B, along with a Borrow-in (Bin) input, and produces two outputs: Difference and Borrow-out (Bout). The design is based on CMOS logic gates, including XOR, AND, and OR gates, to implement the subtraction operation. The subtractor works by applying the 2's complement method for binary subtraction, where the Borrow-in represents the carry-over from previous bits. The schematic illustrates how these gates are connected to achieve the correct difference and borrow outputs for all possible input combinations. The CMOS-based design ensures low power consumption and high-speed operation, making it suitable for efficient digital processing in the 4-bit ALU.
                       
<img width="477" height="495" alt="image" src="https://github.com/user-attachments/assets/0c7ee4c9-3a2c-432b-a653-3e0bc7829582" />

Schematic of the 4-bit magnitude comparator                             

<img width="311" height="575" alt="image" src="https://github.com/user-attachments/assets/6a3e066a-a628-4a3c-a9e5-8710f2a13d75" />

layout of the 4-bit magnitude comparator

The image above illustrates the schematic diagram of the 4-bit magnitude comparator designed using 90nm CMOS technology. This comparator takes two 4-bit inputs, A and B, and compares their values to determine whether A is greater than, less than, or equal to B. The circuit is implemented using basic CMOS logic gates such as AND, OR, and NOT gates, which are arranged to produce three output signals: A > B, A < B, and A = B. These outputs indicate the result of the comparison between the two 4-bit inputs. The schematic showcases how these gates are interconnected to perform the magnitude comparison efficiently. This design ensures accurate and reliable comparison of binary numbers, which is a key component in various arithmetic and logical operations within the 4-bit ALU.
 
<img width="945" height="410" alt="image" src="https://github.com/user-attachments/assets/5a6e40a9-1b41-4b58-a1e3-325bac502837" />

Schematic of the 4-bit one’s complement

<img width="720" height="455" alt="image" src="https://github.com/user-attachments/assets/96783b1a-05f9-4300-95ee-acb95227063c" />

layout of the 4-bit one’s complement

The image above is a schematic design and layout of a 4-bit One’s Complement circuit using four inverters. The design consists of a simple yet effective implementation where each bit of the 4-bit input is inverted using a dedicated CMOS inverter to generate its complement. The schematic was created using 90nm CMOS technology, ensuring optimized performance and minimal power consumption. After designing the circuit, a testbench was developed to verify its functionality through transient analysis, confirming that each input bit correctly flips to its complement. The simulation results validate the expected behaviour, demonstrating the feasibility of this approach for basic arithmetic and logical operations in digital circuits.
 
 <img width="318" height="661" alt="image" src="https://github.com/user-attachments/assets/c783ff91-a36f-40d9-96a9-53696631f5a1" />

Schematic of the 3:8 decoder

<img width="279" height="617" alt="image" src="https://github.com/user-attachments/assets/ffb5f01a-5fcc-4401-aa71-a84c207ac0ef" />

 layout of the 3:8 decoder

The image above is schematic diagram of a 3-to-8 decoder using logic gates in Cadence Virtuoso. The circuit takes a 3-bit binary input and generates eight unique output lines, where each output corresponds to one of the possible input combinations. The design was implemented using AND and NOT gates, ensuring correct decoding logic while maintaining minimal propagation delay. The schematic was developed using 90nm CMOS technology, optimizing power and area efficiency. A testbench was created to verify the functionality through transient analysis, confirming that each output line is activated exclusively based on the input combination. The simulation results validate the expected operation, making this design suitable for applications in memory address decoding and control logic circuits.

<img width="554" height="564" alt="image" src="https://github.com/user-attachments/assets/facd8042-8d17-4e0e-9ad9-a2161aa28877" />

Schematic of the 8:1 Mux			       

<img width="365" height="674" alt="image" src="https://github.com/user-attachments/assets/7e624a11-6056-48a0-860d-eb34cd4d9d98" />

Layout of the 8:1 Mux

The image about is the schematic diagram and layout of an 8:1 multiplexer (MUX) using seven 2:1 multiplexer in Cadence Virtuoso. The hierarchical design follows a tree-like structure, where the first stage consists of four 2:1 MUX selecting between input signals, the second stage has two 2:1 MUX selecting between the first stage outputs, and the final stage uses one 2:1 MUX to produce the final selected output based on the 3-bit select lines. The design was implemented using 90nm CMOS technology, ensuring efficient switching performance with minimal delay. The simulation results validate the expected behaviour, demonstrating the reliability of this design for digital signal selection and data routing applications.

<img width="944" height="350" alt="image" src="https://github.com/user-attachments/assets/de61d96f-bbb5-476a-a2fc-9ea1abad1a3f" />

Schematic of the 4-bit ALU

<img width="943" height="479" alt="image" src="https://github.com/user-attachments/assets/3af6fb46-7f69-45b1-bc43-ff959e11e78e" />

FULL LAYOUT

<img width="653" height="727" alt="custom_layout" src="https://github.com/user-attachments/assets/ba56d229-6221-4df3-bd20-6938e9666f74" />

 layout of the 4-bit ALU

The above images show the schematic diagram and layout design of a 4-bit Arithmetic Logic Unit (ALU) in Cadence Virtuoso, implementing basic arithmetic and logical operations. The ALU takes two 4-bit operands and a set of control signals to perform operations such as addition, subtraction, magnitude comparison, ones complement and 3:8 decoder. The design was implemented using 90nm CMOS technology, ensuring optimized performance in terms of speed and power consumption. The design includes 8 8:1 mux for the control of all output. The simulation results validate the expected behaviour, demonstrating the efficiency and accuracy of this ALU for fundamental computing tasks in digital processing applications.
