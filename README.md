## PIC16F877A-OutputControl-Projects

Here are three smaller tasks (projects). The projects are based on systems that we use in our daily lives, such as traffic lights, staircase automation, etc.

<br>

## LED Running Light

This project is developed using the PIC16F877A microcontroller, designed to control a sequence of LEDs connected to PORTB. Below are the key features and functionalities of the code:

## Features

1. **LED Control**: The program controls multiple LEDs, lighting them in pairs to create a visual effect.

2. **Sequential Lighting**: 
   - LEDs are turned on in a specific sequence:
     - First and last LED
     - Second and seventh LED
     - Third and sixth LED
     - Fourth and fifth LED
   - This creates a dynamic pattern that can be visually engaging.

3. **Timing Control**:
   - Each LED pair is illuminated for 200 ms.
   - The last two sequences are displayed for 500 ms to enhance visibility.

4. **Port Configuration**:
   - PORTB is configured as an output port to drive the LEDs.
   - The initial state of all LEDs is turned off.

5. **Infinite Loop**: The main function runs in an infinite loop, allowing the LED sequence to repeat continuously.

6. **Basic Interrupt Structure**:
   - A placeholder for an interrupt service routine (`MX_INTERRUPT_MACRO`) is defined, indicating the potential for future enhancements such as interrupt-driven events.

<br><br>

## Staircase Light Controller

This project is developed using the PIC16F877A microcontroller, designed to control an LED based on input from a pin connected to PORTA. Below are the key features and functionalities of the code.

## Features

1. **Initialization**:
   - The ADC configuration is set, and the interrupt initialization code is prepared.

2. **Port Configuration**:
   - PORTB is configured to control an LED. The initial state of the LED is turned off.
   - TRISB is set to configure the relevant pins for output.

3. **Input Handling**:
   - The code reads input from RA0 to determine the start signal.
   - If the start signal is detected (i.e., RA0 is high), the LED on PORTB will be turned on.

4. **Output Control**:
   - If the start signal is not detected, the LED will be turned off.
   - The LED's state is updated based on the input received from PORTA.

5. **Timing Control**:
   - When the start signal is not detected, the program pauses for 5 seconds before re-evaluating the input state.

6. **Infinite Loop**:
   - The main function runs in an infinite loop, continuously checking the input state and updating the LED accordingly.

7. **Basic Structure**:
   - The code includes a basic structure for decision-making based on the input from PORTA, allowing for simple control of the LED based on external signals.

<br><br>


## Traffic Light Control System with PIC16F877A

This project is developed using the PIC16F877A microcontroller to control a traffic light system with specific timing sequences for each light (red, yellow, green) connected to PORTA. Below are the key features and functionalities of the code:

## Features

1. **Initialization**:
   - The ADC configuration is set, and the interrupt initialization code is prepared for future enhancements.

2. **Port Configuration**:
   - PORTA is configured to control the traffic light LEDs. The initial state of all lights is set to off.

3. **Traffic Light Control Sequence**:
   - The program manages the state of three traffic lights (A0 for red, A1 for yellow, and A2 for green) with specific timing:
     - **Red Light (A0)**:
       - Turns on and stays illuminated for 3 seconds to signal vehicles to stop.
     - **Green Light (A2)**:
       - Turns on and remains illuminated for a designated period to allow vehicles to proceed.
     - **Yellow Light (A1)**:
       - Activates before the red light to signal a change, staying on for 2 seconds.

4. **Timing Control**:
   - The program includes delays to manage how long each light remains in its current state:
     - The red light is activated for 3 seconds.
     - The green light has a variable duration (you can set this as needed).
     - The yellow light is activated for 2 seconds before switching to red.

5. **Infinite Loop**:
   - The main function runs in an infinite loop, allowing the traffic light sequence to repeat continuously, ensuring a consistent flow of traffic control.

6. **Basic Interrupt Structure**:
   - A placeholder for an interrupt service routine (`MX_INTERRUPT_MACRO`) is defined, indicating the potential for future enhancements such as interrupt-driven events.

This program demonstrates a fundamental approach to traffic light management using the PIC16F877A microcontroller, providing a practical application for controlling vehicle flow at intersections.

<br><br>

## User Interface Examples
<p align="center">
    <img width="600" alt="Screenshot_1" src="https://github.com/user-attachments/assets/1d23dd1a-e12a-434d-a63a-3b3f4785e2c2">
    <br><br>
    Figure 1: Simulation of Traffic Light Using PIC16F877A (Flowcode)
</p>

<p align="center">
    <img width="600" alt="trc1" src="https://github.com/user-attachments/assets/bf67de8b-3f1d-4d76-a62f-be72dfca9c0a">
    <br><br>
    Figure 2: LED Running Light Simulation
</p>

<p align="center">
    <img width="600" alt="trc2" src="https://github.com/user-attachments/assets/099107cc-dc01-4f0d-bc69-9ea867562546">
    <br><br>
    Figure 3: LED Running Light Simulation (Extension)
</p>

<p align="center">
    <img width="600" alt="stubisni automat" src="https://github.com/user-attachments/assets/f29a2e70-b04a-4d2a-b72b-2fe0d3b624d2">
    <br><br>
    Figure 4: Simulation of Staircase Light Controller (Light)
</p>
<br>

## 🧰 Languages & Tools 

<div style="display: inline;">
    <img src="https://skillicons.dev/icons?i=cpp"style="margin-right: 10px;" />
    <img src="https://github.com/user-attachments/assets/cf1d8532-3d73-4eed-9139-c02b9aa10ddb" width="65" height="65" &nbsp; &nbsp;/>
    <img src="https://github.com/user-attachments/assets/906cc158-0e38-420f-b0b4-64fc227677e7" width="65" height="65" &nbsp; &nbsp;/>

</div>



