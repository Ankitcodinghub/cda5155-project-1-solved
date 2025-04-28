# cda5155-project-1-solved
**TO GET THIS SOLUTION VISIT:** [CDA5155 Project 1 Solved](https://www.ankitcodinghub.com/product/cda5155-project-1-solved-2/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;118596&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;2&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (2 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;CDA5155 Project 1 Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 138px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            5/5 - (2 votes)    </div>
    </div>
In this project you will create a simple RISC-V simulator which will perform the following two tasks. Please develop your project in one (C, C++, Java or Python) source file to avoid the stress of combining multiple files before submission and making sure it still works correctly.

• Load a specified RISC-V text file and generate the assembly code equivalent to the input file (disassembler). Please see the sample input file and disassembly output in the project assignment.

• Generate the instruction-by-instruction simulation of the RISC-V code (simulator). It should also produce/print the contents of registers and data memories after execution of each instruction. Please see the sample simulation output file in the project assignment.

You do not have to implement any exception or interrupt handling for this project. We will use only valid testcases that will not create any exceptions. Please go through this document first, and then view the sample input/output files in the project assignment, before you start implementing the project.

Instructions

You can refer to RISC-V Instruction Set Architecture (riscv-ISA.pdf in the course website) to see the format for each instruction and pay attention to the following changes. For example, we introduced a break instruction, modified the opcode format, etc. In other words, you should exactly follow the details from riscv-ISA.pdf except the changes outlined in this document. In this project, we will be using the instruction format from Figure A.23 and A.24 in the book (slide 47 of instruction.pptx).

Your disassembler &amp; simulator need to support the three categories of instructions shown in Figure 1.

Category-1 Category-2 Category-3 Category-4

beq, bne, blt, sw add, sub, and, or addi, andi, ori, sll, sra, lw jal, break

Figure 1: Three categories of instructions

The format of Category-1 instructions is described in Figure 2. It has the same format as the S-type instruction in slide 47 in instruction.pptx except the rightmost two bits. If the instruction belongs to

Category-1, the rightmost two bits (least significant bits) are always “00” preceded by 5 bits Opcode. Note that instead of using 7 bits opcode in RISC-V, we use 5 bits opcode as described in Figure 3. Assume func3 as “000”.

imm[11:5] rs2 rs1 func3 imm[4:0] Opcode (5 bits) 00

Figure 2: Format of Instructions in Category-1

Instruction Opcode

beq 00000

bne 00001

blt 00010

sw 00011

Figure 3: Opcode for Category-1 instructions

If the instruction belongs to Category-2 which has the form “dest ← src1 op src2”, the rightmost two bits (least significant bits) are always “01” as shown in Figure 4. It has the same format as the R-type instruction in slide 47 in instruction.pptx except the rightmost two bits. Then the preceeding 5 bits serve as opcode as listed in Figure 5. Assume func3 as “000” and func7 as “0000000”.

func7 rs2 rs1 func3 rd Opcode (5 bits) 01

Figure 4: Format of Category-2 instructions where both sources are registers

Instruction Opcode

add 00000

sub 00001

and 00010

or 00011

Figure 5: Opcode for Category-2 instructions

If the instruction belongs to Category-3 which has the form “dest ← src1 op immediate_value”, the rightmost two bits (least significant bits) are always “10”. It has the same format as the I-type instruction in slide 47 in instruction.pptx except the rightmost two bits. Then 5 bits for opcode as indicated in Figure 6. The instruction format is shown in Figure 7. Assume func3 as “000”.

Instruction Opcode

addi 00000

andi 00001

ori 00010

sll 00011

sra 00100

lw 00101

Figure 6: Opcode for Category-3 instructions

imm[11:0] rs1 func3 rd Opcode (5 bits) 10

Figure 7: Format of Category-3 instructions with source2 as immediate value

If the instruction belongs to Category-4, the rightmost two bits (least significant bits) are always “11”. Then 5 bits for opcode as indicated in Figure 8. The instruction format is shown in Figure 9. It has the same format as the U-type instruction in slide 47 in instruction.pptx except the rightmost two bits. Also note that the U-type format in the slide shows “imm[31:12]” but we show it as “imm[19:0]” – both means the same as 20-bit immediate value. Finally, we use the full functionality of “jal” (i.e., not assuming rd as x0).

Instruction Opcode

jal 00000

break 11111

Figure 8: Opcode for Category-4 instructions

imm [19:0] rd Opcode (5 bits) 11

Figure 9: Format of Category-4 instructions

All signed numbers should be interpreted using 2’s complement arithmetic. Note that the signed numbers can be in registers, data memories or inside an instruction (e.g., the immediate field is signed for addi). Most importantly, each location (register or data memory) can be treated differently based on the context. For example, an arithmetic instruction (e.g., add) will treat the content of a register as a signed number (in 2’s complement arithmetic), whereas a logical operation (e.g., and) will treat the same register content as an unsigned number (sequence of bits). Please go through riscv-ISA.pdf to understand how each instruction treats its operands (signed or unsigned). Assume that all unassigned register and data memory locations are 0.

Sample Input/output Files

Your program will be given a text input file (see sample.txt). This file will contain a sequence of 32-bit instruction words starting at address “256”. The final instruction in the sequence of instructions is always break. There will be only one break instruction. Following the break instruction (immediately after break), there is a sequence of 32-bit 2’s complement signed integers for the program data up to the end of the file. The newline character can be either “ ” (linux) or “ ” (windows). Your code should work for both cases. Please download the sample input/output files using “Save As” instead of using copy/paste of the content.

Your RISC-V simulator (with executable name as Vsim) should accept an input file (inputfilename.txt) in the following command format and produce two output files in the same directory: disassembly.txt (contains disassembled output) and simulation.txt (contains the simulation trace). Please hardcode the names of the output files. Please do not hardcode the input filename. It will be specified when running your program. For example, it can be “sample.txt” or “test.txt”. Vsim inputfilename.txt

Correct handling of the sample input file (with possible different data values) will be used to determine

60% of the credit. The remaining 40% will be determined from other valid test cases that you will not have access prior to grading. It is recommended that you construct your own sample input files with which to further test your disassembler/simulator. It is okay to share your new testcases with other students in the class as long as it does not lead to similarity in the project source code.

The disassembler output file should contain 3 columns of data with each column separated by one tab character (‘ ’ or char(9)). See the sample disassembly file in the project1 assignment.

1. The text (e.g., 0’s and 1’s) string representing the 32-bit data word at that location.

2. The address (in decimal) of that location

3. The disassembled instruction.

Note, if you are displaying an instruction, the third column should contain every part of the instruction, with each argument separated by a comma and then a space (“, ”).

The simulation output file should have the following format.

20 hyphens and a new line

Cycle &lt; cycleNumber &gt;:&lt; tab &gt;&lt; instr_Address &gt;&lt; tab &gt;&lt; instr_string &gt;

&lt; blank_line &gt;

Registers x00: &lt; tab &gt;&lt; int(x0) &gt;&lt; tab &gt;&lt; int(x1) &gt;…&lt; tab &gt;&lt; int(x7) &gt;

x08: &lt; tab &gt;&lt; int(x8) &gt;&lt; tab &gt;&lt; int(x9) &gt;…&lt; tab &gt;&lt; int(x15) &gt;

x16: &lt; tab &gt;&lt; int(x16) &gt;&lt; tab &gt;&lt; int(x17) &gt;…&lt; tab &gt;&lt; int(x23) &gt;

x24: &lt; tab &gt;&lt; int(x24) &gt;&lt; tab &gt;&lt; int(x25) &gt;…&lt; tab &gt;&lt; int(x31) &gt;

&lt; blank_line &gt;

Data

&lt; firstDataAddress &gt;: &lt; tab &gt;&lt; display 8 data words as integers with tabs in between &gt; ….. &lt; continue until the last data word &gt;

Display all integer values in decimal. Immediate values should be preceded by a “#” symbol. Note that some instructions take signed immediate values while others take unsigned immediate values. You will have to make sure you properly display a signed or unsigned value depending on the context.

Because we will be using “diff –w -B” to check your output versus the expected outputs, please follow the output formatting. Mismatches will be treated as wrong output and will lead to score penalty.

The project assignment contains the following sample programs/files to test your disassembler/simulator.

• sample.txt : This is the input to your program.

• sample_disassembly.txt : This is what your program should produce as disassembled output.

• sample_simulation.txt : This is what your program should output as simulation trace.

Submission Policy:

Please follow the submission policy outlined below. There can be up to 10% score penalty based on the nature of submission policy violations.

1. Please develop your project in one source file. In other words, you cannot submit your project if you have designed it using multiple source files. Please add “.txt” at the end of your filename. Your file name must be Vsim (e.g., Vsim.c.txt or V.cpp.txt or V.java.txt or Vsim.py.txt).

2. Please test your submission. These are the exact steps we will follow too.

o Download your submission from eLearning (ensures your upload was successful).

o Please compile to produce an executable named Vsim.

▪ gcc Vsim.c –o Vsim or javac Vsim.java or g++ -std=c++17 Vsim.cpp –o Vsim o Please do not print anything on screen.

o Please do not hardcode input filename, accept it as a command line option. You should hardcode your output filenames. Execution should always produce disassembly.txt and simulation.txt irrespective of the input filename.

o Execute to generate disassembly and simulation files and test with correct/provided ones

▪ ./Vsim inputfilename.txt or java Vsim inputfilename.txt or ./Vsim.py inputfilename.txt or python3 Vsim.py inputfilename.txt

▪ diff –w –B disassembly.txt sample_disassembly.txt

▪ diff –w –B simulation.txt sample_simulation.txt
