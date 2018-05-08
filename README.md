# FPGA Hardware Emulation of Nintendo Entertainment System (NES)

## Description
Creating an FPGA implementation of the NES in SystemVerilog

## Information
In 1985 Nintendo released a revolutionary gaming console called the NES (Nintendo Entertainment System). The NES was the first true color console to be released, and featured a 6-bit color scheme. This, coupled with other state of the art features, led the console to sell millions of units and become one of the most emulated consoles in history.

The FPGA NES aims to recreate the original feel of the NES while also improving the outputs to modern interfaces. Using Xilinx’s Vivado, SystemVerilog instructs the compiler on how to synthesize the design. The program then creates the digital logic gates and places/routes them to make an actionable circuit.

For the project we selected Digilent’s Zybo Zynq-7010 Development board due to the onboard FPGA’s capabilities as well as the peripheral connections it had available. The Zynq-7010 integrates a dual-core ARM processor with a Xilinx -7 FPGA which allowed for in-depth debugging of the design’s operation.

The project was divided into three major subsystems with two additional sections that were worked on in unison. These components are the Central Processing Unit (CPU), Audio Processing Unit (APU), and the Picture Processing Unit (PPU) along with the minor sections being the Controllers and the Memory Mappers. The CPU takes the data from the cartridges and converts it into actionable instructions that are passed through to the APU and PPU. The APU takes these instructions and uses its four channels to produce 8-bit audio and the PPU uses them to create the sprites and background to be outputted as a video signal.

## Equipment
* Digilent Zybo Zynq-7010 Development Board
* NES Controllers
* NES Controller breakout boards
* 3.5 mm breakout board
* SD card

## Finished product
![alt text](https://github.com/BW0ng/FPGA-NES/raw/master/finished_product.jpg)

## [Final Report](https://docs.google.com/document/d/1TDs1-73mg8NffsuH-0fZAMAmAXpyg7S5ryAIiElqUD8/edit?usp=sharing)

## Authors
* Alexander Underwood
* Brandon Wong
* Clay Patterson
* Daniel Bothwell

For more details please contact Dr. James Stine at james.stine@okstate.edu.
