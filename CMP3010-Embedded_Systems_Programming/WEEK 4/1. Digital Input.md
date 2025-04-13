Basically the bit values of the pins in input ports. You can change these using switches, to make it form 0 to 1 or 1 to 0.
![[Pasted image 20250310131421.png]]

You can check if a switch is pressed by using digitalRead(0), if the value is 1 it is pressed, and if it 0 it is not pressed.

Because of the nature of mechanical parts, the electrical value of the switch can fluctuate, and if it was 0 for a long time it can "bounce" when suddenly turned to 1. 

![[Pasted image 20250310131713.png]]

To solve these problems one would use debouncer circuits:

![[Pasted image 20250310131750.png]]

There is also software solutions, like:
- Delay: Wait a bit before measuring
- Counter: Count input states and average
- Shift Register: Search for the pattern (maybe it rises rises falls 110110110)


