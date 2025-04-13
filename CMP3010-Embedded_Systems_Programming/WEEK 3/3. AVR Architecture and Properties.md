An **AVR microcontroller** is a type of microcontroller developed by **Atmel** (now owned by **Microchip Technology**). AVR microcontrollers are widely used in embedded systems, robotics, and DIY electronics projects due to their ease of use, efficiency, and support from a large developer community.
(Note: AVR doesn’t officially stand for anything. However, according to the original creators at **Atmel**, the name **AVR** was chosen as an internal project codename and doesn’t have a specific meaning.)

![[Pasted image 20250305130322.png]]
###### Breakdown of Components:
1. **CPU (Central Processing Unit)**:
    - The core of the microcontroller that executes instructions and processes data.
    - Connected to both the **Program Bus** and **Data Bus**.
    
2. **Program Flash ROM**:
    - Stores the program code (firmware) that the CPU executes.
    - Connected to the CPU via the **Program Bus**.
    
3. **RAM (Random Access Memory)**:
    - Temporary memory used to store variables and runtime data.
    - Connected to the **Data Bus** for fast access.
    
4. **EEPROM (Electrically Erasable Programmable Read-Only Memory)**:
    - Non-volatile memory used for storing data that must be retained after power loss.
    - Also connected to the **Data Bus**.
    
5. **Timers**:
    - Used for time-related operations such as delays, counting, and generating PWM signals.
    - Interfaced via the **Data Bus**.
    
6. **Ports (I/O Pins)**:
    - Allow interaction with external devices like LEDs, sensors, and motors.
    - Controlled via the **Data Bus**.
    
7. **Interrupt Unit**:
    - Handles interrupts, which allow the microcontroller to respond to external events (like button presses) quickly.
    
8. **Other Peripherals**:
    - Can include additional modules like ADC (Analog-to-Digital Converter), UART (Serial Communication), SPI, I2C, etc.
    
9. **OSC (Oscillator)**:
    - Provides the clock signal necessary for the CPU and other components to function in a synchronized manner.

### How It Works:

- The **CPU fetches instructions** from **Program Flash ROM** via the **Program Bus**.
- It processes data stored in **RAM** or fetched from **EEPROM**.
- It communicates with **timers, interrupts, and peripherals** via the **Data Bus**.
- The **ports** allow input and output operations through **I/O pins**


![[Pasted image 20250305130727.png]]

Memory:
- Flash (32K and 15 bit addresses)
	- Program memory, read only
	- Non volatile
	- Allocate using PROGMEM
- SRAM (2K)
	- Temporary values like stack
	- Volatile
	- Very limited space
- EEPROM (1K)
	- Only for long term data

![[Pasted image 20250305130850.png]]

![[Pasted image 20250305131026.png]]


Port Special Functions:
- Clock connections
- Timer connections
- Interrupts
- Analog references
- Serial bus I/Os
- USART
- PCI

I/O Ports:
- 3 8bit ports (lets call it B, C, D)
	- Separate entities, can modify one port without affecting other
- Each port controlled by 3 8bit registers
	- Each bit controls one pin
	- DDRx - Direction register
		- Defines whether the pin is an input or output pin
	- PINx - Pin input value
		- Reading this register returns the value of pin
	- PORTx - Pin output value
		- Writing this register sets the value of the pin
