# Project_Template

## Team Name: 
ASIC VMA
## Team Members:
- Rithani Priyanga Coimbatore Kannan (hwu6hc)
- Vishnuvartthan Govindaraj (fpp6vt)
  
## Project Title:
ASIC VMA

## Project Description:
(Provide a short description of the problem you're addressing)

## Key Objectives:
To evaluate and list out how Large Language Models, LLMs, such as ChatGPT can assist in various phases of ASIC digital design. Specifically, the project investigates prompting strategies for:

- RTL generation
- Design scaling
- Algorithm-to-HDL conversion
- Module integration
- Testbench generation and verification
- Timing constraint (SDC) file generation

And, to explore how these prompting techniques impact workflow efficiency, correctness, and synthesis performance within industry-standard toolchains like Synopsys Design Compiler and VCS. The effectiveness of each strategy will be evaluated based on:

- Functional correctness
- Synthesis performance (area, timing, power)
- Workflow automation and manual intervention required


## Technology Stack:
- Synopsys Design Compiler, VCS, Primtime
- ChatGPT / Claude
- Linux server
- Python, Verilog, SV, TCL


## Expected Outcomes:
- Comparison of 4+ LLM prompting techniques on one hardware module, VMA
- Synthesis and timing reports via Design Compiler & Primetime
- A metrics based evaluation table (correctness, quality, automation)
- Analysis of LLM-generated constraint files (SDC)
- A report summarizing best practices and limitations of using LLMs for ASIC

## Tasks:

#### Rithani

- Define the MAC architecture (2, 4, 8 elements)
- Run synthesis using Design Compiler
- Simulate LLM-generated RTL and testbenches using VCS
- Analyze simulation outputs and verify correctness

#### Vishnu

- Prompt ChatGPT or Claude to generate base RTL for the MAC unit, MAC algorithm from C to Verilog, scale MAC design from 2 to 8 elements 
- Prompt to integrate MAC module into a larger datapath, to generate Verilog testbenches and timing constraint files
- Perform timing analysis using Primetime
- Compiling the evaluation report, including the parts for design flow that LLMs can be integrated, and the quality of the program with different strategies


## Timeline:
#### Week 1
- Finalize the number of elements (2 → 8) for scalability testing.
- Create a block diagram of the architecture.
- Run basic simulations to check if the RTL compiles and works as expected
- If issues found, refine the prompting strategy for improved RTL output.


#### Week 2: Scaling, Integration, Testbenches, and Timing Constraints
- Scale the 2-element MAC to a 4-element MAC and then to 8-element.
- Integrate the MAC into a larger datapath (if applicable).
- Generate testbenches, timing constraints, and perform the first round of simulations, Verilog testbench to verify this MAC module with random input values for 8-element MAC, a valid SDC file.
- Verify the functionality of both the design and testbench.
- Check if the synthesized design meets the basic area/timing requirements.

#### Week 3: Final Analysis
- Verifying if the timing constraints are met post-synthesis and addressing any timing issues.
- Discuss integration strategies, workflow improvement, and the effectiveness of LLMs in each phase (RTL generation, scaling, testbenches, constraints).
- Evaluate the quality of the LLM generated outputs, like the correctness, efficiency, and synthesis performance.
- Final testing on the complete design, including full verification with the testbench and synthesis/timing reports, and highlighting the key findings, results, and conclusions about the use of LLMs in ASIC design.


