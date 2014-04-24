Lab5_Wooden
===========

The Prisim design in VHDL and FPGA


Part One: I had Dr. Neebel check my functionality at the begining of class on lesson 33. I recieved full credit on functionality
for Part 1.

Part Two: I had Captain Silva check off my part two functionality, in which I recieved full points.


##Part One Discussion

The purpose of part one was to connect our ALU to the datapath to create a funcitoning PRISM model in VHDL.

Once the ALU was connect we could easily run the ROM file that we wished to execute from the PRISM code.

The Lab5 handout gave us a picture of what the code was supposed to do so that we could make sure the VHDL was functioning
properly.

![alt text](https://raw.githubusercontent.com/JarrodWooden/Lab5_Wooden/master/to50ns.PNG "First 50 nano seconds")

The first 50ns shows that it is following what it is supposed to be doing from the PRISM code given to us from the Lab5 
handout.

![alt text](https://raw.githubusercontent.com/JarrodWooden/Lab5_Wooden/master/to85ns.PNG "85 nano seconds")

Then after 8 is added in 1 is added immediately which makes the current value in the accumulator nine.

![alt text](https://raw.githubusercontent.com/JarrodWooden/Lab5_Wooden/master/to130ns.PNG "135 nano seconds")

Then this portion of the simulation shows the output of the accumulator to the output pin

![alt text](https://raw.githubusercontent.com/JarrodWooden/Lab5_Wooden/master/to175ns.PNG "180 nano seconds")

Finally the picture above shows how the program is about to jump to the beginning of the loop.

After I declared and instantiated my PRISM module inside the `Nexys2_top_shell.vhd` file I was able to compile the
code in VHL and program the code to the FPGA.

I was able to get the functionaly checked off once the FPGA was programmed.

##Part Two

The objective to part two was that we were given a design prompt that we were supposed to code using the PRISM assembly
code. Once the program was coded in the PRISM simulation and working properly we could save the ROM file and upload the
program to the Datapath we made from part one to be able to program Part Two to the FPGA.

The Prism Code is above so you can see for yourself how I coded the prompt. The prompt is below:

"1. Output a two digit number on Output Ports 1 and 2. 
2. The output value will count up through decimal values 00 ► 01 ► 02 ….. 98 ► 99 ► 00.
3. If at any time the user enters a hexadecimal number in the range 8 – F on Input Port 0, the count pattern will change
    such that it will count down from the current value. 
4. If at any time the user enters a hexadecimal number in the range 0 – 7 on Input Port 0, the count pattern will change     back to a count up pattern. 
5. Please note, the Input Port has nothing to do with the value of the counter, it ONLY controls the direction of the 
    count."

I was able to get this by going through systematically and creating loops for specific functions that I knew were going
to have to be repeated multiple times throughout the code. Once I got it working I was able to save the ROM file
to the Lab folder and use the ROM file to implement the code in VHDL and program my FPGA.

Once I was able to get the code working properly on the FPGA I was able to get checked off for my product's functionality.

##Cool things with Inputs and Outputs

What I did for my cool things with inputs and outputs was that I took in all four inputs from the input pins and simply
doubled them to be the output for the output pins.

Once the inputs were doubled the code simply keeps adding one over and over again to the doubled numbers in the output
in an infinite loop. I thought it was pretty NEAT.

Thank you for reading my ReadME

#Have a Great Air Force Day!!!!



