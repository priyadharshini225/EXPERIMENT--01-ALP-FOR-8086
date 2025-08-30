# EXPERIMENT--01-ALP-FOR-8086
 Name : PRIYADHARSHINI S
 
 Roll no : 212223240129

 Date of experiment : 30/08/2025





## Aim: To Write and execute ALP on fundamental arithmetic and logical operations
## Components required: 8086  emulator 
## Theory 
Running The Emulator (emu8086) Intro 8086 Microprocessor Emulator, also known as EMU8086, is an emulator of the program 8086 microprocessor. It is developed with a built-in 8086 assembler. This application is able to run programs on both PC desktops and laptops. This tool is primarily designed to copy or emulate hardware. These include the memory of a program, CPU, RAM, input and output devices, and even the display screen. There are instructions to follow when using this emulator. It can be executed into one of the two ways: backward or forward. There are also examples of assembly source code included. With this, it allows the programming of assembly language, reverse engineering, hardware architecture, and creating miniature operating system (OS). The user interface of 8086 Microprocessor Emulator is simple and easy to manage. There are five major buttons with icons and titles included. These are “Load”, “Reload”, “Step Back”, “Single Step”, and “Run”. Above those buttons is the menu that includes “File”, “View”, “Virtual Devices”, “Virtual Drive”, and “Help”. Below the buttons is a series of choices that are usually in numbers and codes. At the leftmost part is an area called “Registers” with an indication of either “H” or “L”. The other side is divided into two, which enables users to manually reset, debug, flag, etc. What is 8086 emulator emu8086 is an emulator of Intel 8086 (AMD compatible) microprocessor with integrated 8086 assembler and tutorials for beginners. Emulator runs programs like the real microprocessor in step-by-step mode. it shows registers, memory, stack, variables and flags.


 ## Running the Emulator :
1.	Download and install emu8086 (www.emu8086.com) It is usually installed in C:\EMU8086 subfolder in the “Windows” directory
2.	  Run  emu8086 icon (on the desktop or in the c:\EMU8086 folder of window) It has green color 
 
 
3.		write the code for the appropriate program for ADDITION,SUBTRACTION, MULTIPLICATION,  DIVISION operations 

4.	 Compile the program and check for the errors 
5.	Run (once there is no syntax error) 

6.	Click OK to see/view the output of your program on the Emulator screen. 


7.	After running the program, another menu screen will be displayed, where you have the option to “View” symbol table,
8.	 


![image](https://user-images.githubusercontent.com/36288975/189273263-d65baae9-4b8f-4723-afb3-c0ffa4052b04.png)











9.	Click on emulate to start emulation 








![image](https://user-images.githubusercontent.com/36288975/189273273-9bb36ec1-e2e8-4892-8d35-37707332bfdc.png)








10.	If no errors are found click on run the program and check the status of various flags in the flags tab as shown below 






![image](https://user-images.githubusercontent.com/36288975/189273277-113a2a33-4a40-4ff8-95a5-ecd3a1f504fe.png)







## Programs for arithmetic  operations

## Addition  of 8 bit ALP 
```
MOV CL,00
MOV AX,[3001H]
MOV BX,[3003H]
ADD AX,BX
JNC Loop
INC CL
Loop:
MOV [3005H],AX
MOV [3007H],CL
HLT 
```

## Output  
<img width="1919" height="1017" alt="1 ADD" src="https://github.com/user-attachments/assets/601943e1-11c2-4c2b-bfb3-1461dd697086" />


 
## Subtraction   of 8 bit numbers  ALP 
```
MOV CL,00
MOV AX,[3001H]
MOV BX,[3003H]
SUB AX,BX
JNC Loop
INC CL  
NOT AX
INC AX
Loop:
MOV [3005H],AX
MOV [3007H],CL
HLT      
```
 
## Output  
<img width="1911" height="1017" alt="2 SUB" src="https://github.com/user-attachments/assets/5c6e4eac-e99e-4d65-9fa6-d6b18c822075" />

## Multiplication alp 
```
MOV AX,[3001H]
MOV BX,[3003H]
MUL BX
MOV [3005H],AX
MOV [3007H],DX
HLT
```
 ## Output  

<img width="1905" height="1014" alt="3 MUL" src="https://github.com/user-attachments/assets/0e45007c-d456-408d-b772-76fefbf1ccf9" />


## Division alp 
```
MOV AX,[3001H]
MOV BX,[3003H]
DIV BX
MOV [3005H],AX
MOV [3007H],DX
HLT
```

## Output  
<img width="1909" height="1016" alt="4 DIV" src="https://github.com/user-attachments/assets/7f4590b0-8771-4a0b-824e-491492f14cee" />

## LOGICAL OPERATIONS

## TRUTH TABLE FOR LOGICAL OPERATIONS

![symbols-truth-tables-of-common-logic-gates](https://github.com/user-attachments/assets/6caae067-aca0-4b9c-83e3-d22429c1b3ec)



## AND alp
```
MOV AX,[3001H]
MOV BX,[3003H]
AND AX,BX
MOV [3005H],AX
HLT
```
## Output
<img width="1903" height="1017" alt="5 AND" src="https://github.com/user-attachments/assets/be13f2d4-3ca7-47f6-a0e0-072557b6eca1" />

## OR alp
```
MOV AX,[3001H]
MOV BX,[3003H]
OR AX,BX
MOV [3005H],AX
HLT
```
## Output
<img width="1907" height="1010" alt="7 OR" src="https://github.com/user-attachments/assets/1cde2cf4-abfb-4626-ac7a-b8bd62a0cd53" />

## NAND alp
```
MOV AX,[3001H]
MOV BX,[3003H]
AND AX,BX
NOT AX
MOV [3005H],AX
HLT
```
## Output
<img width="1902" height="1022" alt="6 NAND" src="https://github.com/user-attachments/assets/039eb0cb-c020-4e83-8ece-ece35cd65014" />

## NOR alp
```
MOV AX,[3001H]
MOV BX,[3003H]
OR AX,BX
NOT AX
MOV [3005H],AX
HLT
```
## Output
<img width="1908" height="1014" alt="8TH NOR" src="https://github.com/user-attachments/assets/68d86f8c-11ff-4aa7-858c-0d1cde714887" />



## NOT alp
```
MOV AX,[3001H]
MOV BX,[3003H]
NOT AX
MOV [3005H],AX
HLT
```
## output
<img width="1910" height="1017" alt="9 NOT" src="https://github.com/user-attachments/assets/19d4a2fc-74b1-496e-8a84-adb7abf10316" />


## XOR alp
```
MOV AX,[3001H]
MOV BX,[3003H]
XOR AX,BX
MOV [3005H],AX
HLT
```
## output
<img width="1910" height="1011" alt="10 XOR" src="https://github.com/user-attachments/assets/6333c93b-28a2-45bf-811d-c83d055a57a5" />


## XNOR alp
```
MOV AX,[3001H]
MOV BX,[3003H]
XOR AX,BX
NOT AX
MOV [3005H],AX
HLT
```
## output
<img width="1910" height="1015" alt="11 XNOR" src="https://github.com/user-attachments/assets/5e183e90-126a-4ffb-931d-8e165f523dbb" />


## Result :
 
The Write and execute ALP on fundamental arithmetic and logical operations is executed successfully.







