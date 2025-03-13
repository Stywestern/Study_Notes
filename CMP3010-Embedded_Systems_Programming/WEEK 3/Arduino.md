
Arduino Uno:
- A microcontroller based on the ATmega328
- 14 digital I/O (6 for PWM)
- 6 analog inputs
- CPU (8 bits) clock: 16 MHz
- Max program size 30Kbytes
- SRAM: 2KB, EEPROM 1KB
- UART, SPI and I2C protocols enabled

![[Pasted image 20250305131752.png]]

Arduino C/C++ Programs
- They are called "sketches", basically Cpp with special libraries
- Program structure:
	- Header: declarations, includes, etc.
	- setup()
	- loop()
- setup()
	- This function executes once when the program starts
- loop() -but like a superloop-
	- Continuously re-executed when the end is reached

e.g.
	int main(void){
		setup();
		for(;;)
			loop();
		return 0; 
		}

Blink Program:
int LedPin = 13 // LED connected to digital pin 13
// setup runs once 
void setup(){
// initialize the pin as output
pinMode(ledPin, OUTPUT);
}
// loop runs over and over again, or as long as Arduino machine has power
void loop(){
digitalWrite(ledPin, HIGH) // open the led
delay(1000) // wait
digitalWrite(ledPin, LOW) // close the led
delay(1000)
}


