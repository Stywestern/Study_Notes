DFA (Deterministic Finite Automata): In this group the machine can exist in only one state at any given time.

NFA (Non-Deterministic Finite Automata): In this group the machine can exist in only one state at any given time.

The key difference between the FNs and the other more powerful types (like Pushdown Automata or Turing Machines) is that FNs have constant memory. 

Widely used in pattern recognition softwares; such as compilers, regular expressions and network protocols designs.

A Deterministic Finite Automaton (DFA) consists of: 
	• Q ==> a finite set of states 
	• ∑ ==> a finite set of input symbols (alphabet) 
	• δ ==> a transition function, which is a mapping between Q x ∑ ==> Q 
	• q0 ==> a start state 
	• F ==> set of accepting states 
	• A DFA is defined by the 5-tuple: • {Q, ∑ , δ, q0, F}

![[Pasted image 20250224125055.png]]

If an alphabet A is the set of all strings that machine M accepts, then A is the language of machine M, denoted L(M) = A. Or it is said M "recognizes" A. 
All machines recognize the "empty language", which only has the empty string. 

In order for a substring s to be accepted by a DFA, no matter which state the machine is in the substring should result in reaching the accepting state:

![[Pasted image 20250224130310.png]]





