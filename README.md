# EXPERIMENT-03-DEVELOPING-COUNTER-LADDER-LOGIC-FOR-PLC-

**NAME:** Akil S 
**REGISTER NUMBER:** 212225220007  
**DEPARTMENT:** B.Tech IT
**YEAR:** 2nd YEAR  

## Aim:
To understand and implement various counter operations in Programmable Logic Controller (PLC) ladder logic.

## Apparatus Required:
- Programmable Logic Controller (PLC): A PLC that supports counter functions. 
- PLC Programming Software: Software such as RSLogix, TIA Portal, or CX-Programmer. 
- Computer System: For programming and simulating the PLC ladder logic. 
- Input Devices: Push buttons or switches to trigger the counter operations. 
- Output Devices: LEDs or other indicators to visualize the counter outputs. 
- Wires and Connectors: For interfacing input/output devices with the PLC. 
- Power Supply: Appropriate power supply for the PLC and peripherals.

## Theory:
Counters in PLCs are used to count events or occurrences, such as the number of items passing on a conveyor belt, the number of cycles a machine runs, or how many times a process has started or stopped. Counters are commonly used in automation to perform tasks like stopping a machine after a set number of products or signaling a notification when a count reaches a specific value.

### Types of Counters:
**Up Counter (CTU) Functionality:**
The up counter counts every time the input condition becomes TRUE (ON). When the accumulated value reaches the preset value, the counter output becomes TRUE. If the reset input is triggered, the counter resets to zero. 

**Down Counter (CTD) Functionality:**
The down counter decreases the count every time the input condition becomes TRUE (ON). When the count reaches zero, the counter output becomes TRUE. The counter can be reset by a reset input to the preset value. 

**Up/Down Counter (CTUD) Functionality:**
The up/down counter can increment or decrement the count based on two different inputs. One input increments the count, while the other decrements it. When the count reaches the preset value or zero, the respective outputs become TRUE. The counter can be reset as required.

## Procedure:
1. **Setup the PLC Programming Environment:** Connect the PLC to the computer and launch the PLC programming software. Ensure all input and output devices are connected to the PLC’s I/O modules. 
2. **Create Ladder Logic for Counters:** 
   - **Up Counter (CTU):** Create a rung with an input (e.g., a push button) linked to a CTU instruction. Set the preset value (e.g., 10 counts). Assign an output to indicate when the preset value is reached. 
   - **Down Counter (CTD):** Create a rung with an input linked to a CTD instruction. Set the preset value (e.g., 5 counts). Assign an output to indicate when the counter reaches zero. 
   - **Up/Down Counter (CTUD):** Create a rung with separate inputs for counting up and counting down. Set the preset value (e.g., 8 counts). Assign outputs for when the count reaches the preset value or zero. 
3. **Simulate the Ladder Logic:** 
   - **Up Counter (CTU):** Run the simulation in the PLC software. Press the input button repeatedly and observe the counter increment until the preset value is reached, at which point the output activates. 
   - **Down Counter (CTD):** Run the simulation, press the input button repeatedly, and observe the counter decrement. When the counter reaches zero, the output activates. 
   - **Up/Down Counter (CTUD):** Simulate both the up and down counting inputs. Observe how the counter increments or decrements and how the output is activated when the count reaches the preset value or zero. 
4. **Download and Execute:** Download the ladder logic program to the PLC if available and run it. Test the counters with the physical push buttons and observe the LEDs or other output devices.

## Outputs:
- **Up Counter (CTU):** The output LED or indicator should activate when the preset count (e.g., 10) is reached. 
- **Down Counter (CTD):** The output should activate when the count reaches zero. 
- **Up/Down Counter (CTUD):** The output should activate when the count reaches the preset value or zero, depending on the inputs.

## Simulation Screenshots:
### COUNTER
<img width="999" height="530" alt="image" src="https://github.com/user-attachments/assets/1e2399f8-1206-4b02-b927-ba40c0461624" />
<img width="1005" height="537" alt="image" src="https://github.com/user-attachments/assets/8e23e23f-bc17-48b2-8d61-850aa2577175" />
<img width="1002" height="529" alt="image" src="https://github.com/user-attachments/assets/0ab72c6c-dcb8-49f7-b8a2-f5dc1dabc1ce" />
<img width="1008" height="523" alt="image" src="https://github.com/user-attachments/assets/ac686663-e2fe-41aa-b3b1-5b060cf6897f" />
<img width="1000" height="532" alt="image" src="https://github.com/user-attachments/assets/218f65fc-e12f-49f5-b833-709733b20405" />
<img width="1009" height="532" alt="image" src="https://github.com/user-attachments/assets/85cc420d-7b9a-43ca-b9e4-b2e2faed77f8" />

### UP COUNTER
<img width="1008" height="536" alt="image" src="https://github.com/user-attachments/assets/0b3ae3a8-c467-4f41-a939-4ea4577fb7c9" />
<img width="1005" height="414" alt="image" src="https://github.com/user-attachments/assets/68916544-fe91-4d6b-801b-a606098861d0" />
<img width="1005" height="444" alt="image" src="https://github.com/user-attachments/assets/8d6ebfb4-085b-4f12-81ac-f792238b6949" />

### DOWN COUNTER
<img width="1000" height="732" alt="image" src="https://github.com/user-attachments/assets/e1b650d6-7f7b-4725-8fcc-91662fe9f2fd" />
<img width="996" height="595" alt="image" src="https://github.com/user-attachments/assets/303c3daa-90b1-45c0-8e85-aa828b509699" />
<img width="998" height="803" alt="image" src="https://github.com/user-attachments/assets/15a1bca0-b1b1-4049-a465-a3b5b94a3188" />
<

### UP/DOWN COUNTER - 1
img width="1005" height="292" alt="image" src="https://github.com/user-attachments/assets/3669bc1b-2418-4f2c-a363-51a380f6ddef" />
<img width="1003" height="534" alt="image" src="https://github.com/user-attachments/assets/c50ae988-c58e-47c0-aa43-8b40490d3ad8" />
<img width="1001" height="534" alt="image" src="https://github.com/user-attachments/assets/34317a1c-fbd6-4b81-a940-547733634766" />
### UP/DOWN COUNTER - 2
<img width="1003" height="529" alt="image" src="https://github.com/user-attachments/assets/0db83e65-8a3b-40f6-bda7-940fe0a4e6d5" />
<img width="1000" height="536" alt="image" src="https://github.com/user-attachments/assets/a5aa730d-4113-4645-abd6-93bba25ad2e2" />
<img width="1003" height="533" alt="image" src="https://github.com/user-attachments/assets/6d2f15de-27f8-4329-851f-f25f46f59fef" />


## Results:
The ladder logic programs for Up Counter (CTU), Down Counter (CTD), and Up/Down Counter (CTUD) were successfully implemented and tested. The outputs behaved as expected, indicating correct counting operations. The experiment demonstrated how counters are essential in automation for counting events and managing process sequences.
