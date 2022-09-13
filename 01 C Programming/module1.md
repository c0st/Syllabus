### CHAPTER 1: MANAGING INPUT AND OUTPUT OPERATIONS
**What is C Language?**

[C](https://en.wikipedia.org/wiki/C_(programming_language)) is a general-purpose computer programming language. It was created in the 1970s by Dennis Ritchie, and remains very widely used and influential.

**Bit, Byte and Words**

- A bit is the smallest unit of information in a computer. It is either a 0 or a 1
- A byte is a group of 8 bits
- A word is a group of 4 bytes
- A nibble is a group of 4 bits

****

Storage | Bits
-- | --
1 Byte | 8
1 Word | 32 or 64
1 Kilo Byte | 1024
1 Mega Byte | 1024 * 1024
1 Giga Byte | 1024 * 1024 * 1024
1 Tera Byte | 1024 * 1024 * 1024 * 1024
1 Peta Byte | 1024 * 1024 * 1024 * 1024 * 1024

**CPU**

![CPU Architecture](https://github.com/c0st/C/blob/main/Drawables/cpu.png)

- CPU is the part of the computer that performs the basic arithmetic, logic, controlling, and input/output (I/O) operations specified by the instructions in a computer program

- `ALU` is a “super calculator” carrying out all arithmetic tasks and Boolean operations
- CU controls the way data is moved between the various components of computer
- Both ALU and CU use the service of clock for synchronizing their operations
- All program instructions are executed using the fetch-decode-execute mechanism. An instruction is first fetched from memory, decoded and then executed by CPU. The CPU can execute one instruction in one clock pulse
- faster the clock, faster is the execution. Todays CPU are rated in GHz

**Memory**

#### RAM (Random Access Memory)

**SRAM (Static RAM)**
- SRAM is a type of memory that retains its data even when the power is turned off. It is faster than DRAM, but more expensive and uses more power
- SRAM is used in CPU cache, memory-mapped I/O

**DRAM (Dynamic RAM)**
- DRAM is a type of memory that loses its data when the power is turned off. It is slower than SRAM, but cheaper and uses less power
- DRAM is used in main memory, video memory

#### ROM (Read Only Memory)
- ROM is a type of memory that retains its data even when the power is turned off. It is used to store the BIOS and other firmware
- `PROM` (Programmable ROM) is a type of ROM that can be programmed once
- `EPROM` (Erasable Programmable Read Only Memory) is a type of ROM that can be erased and reprogrammed once
- `EEPROM` (Electrically Erasable Programmable Read Only Memory) is a type of ROM that can be erased and reprogrammed many times

#### Cache Memory
- It holds those portions of program that are frequently used by CPU
It acts as a buffer between CPU and RAM. The CPU first looks for the instructions in cache.
It executes faster than RAM, expensive and limited in size. It has multiple levels:
- L1 (Level 1) – smallest and fastest – 32 KB
- L2 (Level 2) – present closer to CPU – 256 KB
- L3 (Level 3) – shared by cores – 8 MB

**Speed Comparison**

- Register – fastest – 1 clock cycle
- Cache – faster than RAM – 10 clock cycles
- RAM – slower than cache – 100 clock cycles
- Hard Disk – slowest – 100,000 clock cycles

**Ports**

- Ports are the physical connections on the motherboard that allow the CPU to communicate with other devices
- USB, VGA, HDMI, Ethernet, PS/2, RJ-45, FireWire, Thunderbolt, etc.

**OCR vs MICR**

OCR	| MICR
-- | --
Optical Character Recognition | Magnetic Ink Character Reader.
OCR can scan any kind of printed text | MICR scan specific formats present in a cheque.
A wide variety of fonts are supported | Few fonts are supported like E-138 and CMC-7.
A wide variety of inks are supported | Magnetic ink created using iron oxide, is supported only.
Scanned data is used to edit or print | Scanned data is used to process cheque.

**CRT vs LCD vs LED**

CRT monitors and televisions are traditional monitors. In CRT displays, the image is produced by the firing of electrons from the back of the phosphor tube towards the center of the screen. The phosphorus emits light when heated by the electron, which is then projected onto a screen. The color you see on your screen is made up of a combination of red, blue, and green light sources.

Liquid crystal displays are used to display images on a computer screen using liquid crystal technology. Laptops and flat-panel monitors are common examples of LCD displays. Having improved and continuously advanced over the years, LCD technology is considered the clear leader today.  In terms of color and picture quality, as well as delivering high resolution, it is impressive.

A flat screen or flat-panel computer monitor or television is known as a LED monitor, short for a light emitting diode monitor. These monitors are small and light, with a shallow depth. It is the backlighting that makes this monitor different from a standard LCD. The backlighting is made up of LED lights, which are more energy efficient than the fluorescent lights used in LCD monitors.

Basis | CRT | LCD | LED
-- | -- | -- | --
Represent | Cathode Ray Tube | Liquid Crystal Display“ | Light Emitting Diode
Compounds | Vacuum glass tube, electron gun, phosphor screen,  deflection plates. | Glass plates, internal light source; nematic liquid crystal | Post and Anvil, semiconductor Die, Reflect cavity, epoxy lens
Size | CRTs are bulky, heavy, and large | LCDs are thin, light, and compact | LED is light, compact, and Thinner.
Weight | Heavier | Lighter | Thinner
Power Consumption | High power | Low power | Lower power.
Color | Black | White | True Black.
Image Retention | CRT lacks image retention | LCDs have image retention | It retains images.
Cost | Less expensive | More expensive | Most expensive.
Image Forming | Used Electron Gun | Used Liquid crystals | Used Light Emitting Diode  
Response | Good response | Slow response | Sufficiently fast response.
Benefits | Panels are lighter than plasma; more energy efficient; emits less; thinner; light; radioactive; no bleeding or smearing | Easy to move; picture quality is Good; wide viewing quality; cheaper; multiple resolutions; sharper image quality | Sleek design; Image quality is brighter and sharper; Flicker-free Images; There isn’t any motion delay or lag at all; Larger viewing angle (175 degrees)
Limitations | Film-like picture; slow refresh rate; narrow field of view; blacks and brights; image persistence is possible; pixel death is also possible | Heavy, small displays; outdated technology; easily burnt in | Temperature and age affect the color; LEDs are much thinner; LEDs cost more.
Where Used | Used in old computer monitors and Televisions | Used in flat screens | Used in flat panels display.

#

**Printers**

- **Impact Printers**: It produces the hardcopy of output. The impact printers are old, noisy.
But, still dot-matrix printer is in usage.

- Dot-Matrix Printer: The print head of the dot-matrix printer has either 9 or 24 pins. When the
pins fire against the ribbon, an impression is created on the paper. The speed is 300 cps and
doesn’t produce high quality output. It can produce multiple copies.

- Daisy-wheel Printer: It employs a wheel with separate characters distributed along its outer
edge. The wheels can be changed to obtain different set of fonts.


- Line Printer: For heavy printing, the line printer is used. It uses a print chain containing the
characters. Hammers strike the paper to print and it rotates at the speed of 1200 lpm. It is also
noisy and is of low-quality.

- **Non-Impact Printers**: They are fast, quiet and of high resolution. The most commonly
used non-impact printers are laser and ink-jet printers. The thermal printer is not discussed
here because it uses heat to print on high-sensitive paper.

- Laser Printer: It works like a photocopier and uses toner i.e. black magnetic powder. The image
is created in the form of dots and passed from drums on to the paper. It has built-in RAM which
acts as buffer and RAM to store fonts. The resolution varies from 300 dpi to 1200 dpi and the
speed is about 20 ppm.

- Ink-jet Printer: These are affordable printers. It sprays tiny drops of ink at high pressure as it
moves along the paper. The separate cartridges are available for different colors. The resolution
is about 300 dpi, can print 1 to 6 pages/min.

- Plotters: The plotter can make drawings. It uses one or more automated pens. The
commands are taken from special file called vector graphic files. Depending on type of plotter
either paper or pen moves. It can handle large paper sizes and it is used for creative drawings
like buildings and machines. They are slow and expensive.

**Network Topology**

- Bus Topology: It uses a single cable called as bus to which all computers are connected.
The failure of one single node doesn’t disturb other nodes.

- Star Topology: It uses a central hub to which all nodes are connected. If the hub fails,
entire network fails and the nodes cannot be added easily.

- Ring Topology: It is connected in the form of closed loop without hub. Data moves from
node to node. For unidirectional rings, if one node fails, the network fails.

- Mesh Topology: Nodes are connected to one another offering multiple paths. If node
breaks down, then data passing changes its route. It is expensive

![img](https://github.com/c0st/C/blob/main/Drawables/network.jpg)

#


**Network Types**
- Local Area Network - They are used in smaller organizations usually using
Ethernet. The usual speed will be 100Mbps.

- Wide Area Network - They are used in cities and can connect larger distance.
They use optic fiber cables. Banks, Airline and Hotel reservations use WANs.
- Metropolitan Area Network - It is sandwiched between LAN and WAN and used
for interconnecting in same cities.
- Personal Area Network - This is the smallest network and can connect only few
meters. It connects small devices like phones, laptops through Bluetooth

#

The `Internet` is the set of all networks which are interconnected and interoperate using the IETF standard protocols
An `internet` (lowercase-i) is any network of devices which can communicate with each other

**Software**

System Software | Application Software
-- | --
System software is used for operating computer hardware | Application software is used by user to perform specific task.
System softwares are installed on the computer when operating system is installed | Application softwares are installed according to user’s requirements.
user does not interact with system software because it works in the background | In general, the user interacts with application softwares
System software can run independently. It provides platform for running application softwares | Application software can’t run independently. They can’t run without the presence of system software.
compiler, assembler, debugger, driver | word processor, web browser, media player


### Chapter 2 Overview of C

**Psuedo Code**

Pseudocode is a detailed yet readable description of what a computer program or algorithm must do, expressed in a formally-styled natural language rather than in a programming language. Pseudocode often uses structural conventions of a normal programming language, but is intended for human reading rather than machine reading.

**Tokens**

A token is a sequence of characters that are meaningful to the compiler. Tokens are the smallest meaningful units of a program. Tokens are classified into various categories such as identifiers, keywords, operators, separators, literals, etc.

**Operators**

Operators are special symbols that represent computations like addition, multiplication, and division. The values the operator works on are called operands.

**Arithmetic Operators**

Operator | Description
-- | --
\+ | Addition
\- | Subtraction
\* | Multiplication
/ | Division
% | Modulus
++ | Increment
-- | Decrement

**Relational Operators**

Operator | Description
-- | --
== | Equal to
!= | Not equal to
\> | Greater than
< | Less than
\>= | Greater than or equal to
<= | Less than or equal to

**Logical Operators**

Operator | Description
-- | --
&& | Logical AND
\|\| | Logical OR
! | Logical NOT

**Assignment Operators**

Operator | Description
-- | --
= | Simple assignment
+= | Add AND assignment
-= | Subtract AND assignment
*= | Multiply AND assignment
/= | Divide AND assignment
%= | Modulus AND assignment

**Increment / Decrement operators**

Operator | Description
-- | --
++ | Increment
-- | Decrement

**Bitwise Operators**

Operator | Description
-- | --
& | Bitwise AND
\| | Bitwise OR
^ | Bitwise XOR
~ | Bitwise compliment
<< | Left shift
\>\> | Right shift

**Conditional operator**

**expression1 ? expression2 : expression3**

If expression1 is `true`, then `expression2` is evaluated and becomes the result of the entire conditional expression. If expression1 is `false`, then `expression3` is evaluated and becomes the result of the entire conditional expression.

**Special operator**

Operator | Description
-- | --
sizeof | Returns the size of a variable
& | Returns the address of a variable
\* | Pointer to a variable
?: | Conditional operator
, | Comma operator

****

```
c = (a , b);
>> c = b
c = a , b;
>> c = a
```

**Precedence**


Operator | Description
-- | --
\[\] | Array subscript
\(\) | Function call
. | Structure member
\-\> | Structure pointer member
\+\+ | Increment
\-\- | Decrement
\~ | Bitwise complement
! | Logical complement
\* | Multiply
/ | Divide
% | Modulus
\+ | Add
\- | Subtract
<< | Left shift
\>\> | Right shift
< | Less than
\> | Greater than
<= | Less than or equal to
\>= | Greater than or equal to
== | Equal to
!= | Not equal to
& | Bitwise AND
^ | Bitwise XOR
\| | Bitwise OR
&& | Logical AND
\|\| | Logical OR
?: | Conditional
= | Assignment
\+= | Add and assignment
\-= | Subtract and assignment
\*= | Multiply and assignment
/= | Divide and assignment
%= | Modulus and assignment
<<= | Left shift and assignment
\>\>= | Right shift and assignment
&= | Bitwise AND and assignment
^= | Bitwise XOR and assignment
\|= | Bitwise OR and assignment

**Tips for Programming Errors**

1. Avoid division by zero errors whenever arithmetic expressions are evaluated
2. Use parentheses whenever complex expressions with operators of various Precedence and
Associativity are used
3. Be careful while using increment decrement operators
4. Never give space between relational operators < = , > = , ! = etc.
5. Increment/ decrement operators do not work with floating point numbers.