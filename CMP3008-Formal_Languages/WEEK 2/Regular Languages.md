If language L is recognized by a DFA A than L(A) is called a "Regular Language"

Regular Operations -------
If A and B are languages then:
	Union: A $\cup$ B = {x | x $\in$ A or x $\in$ B}
	Concatenation: A $\circ$ B = {xy | x $\in$ A or x $\in$ B}
	Star: A* = {x1y2...xk | k $\ge$ 0 and each xi $\in$ A}

Example:
![[Pasted image 20250224131229.png]]

Closure under union: If A and B are regular languages than C = A $\cup$ B is also regular.

Closure under concatenation: If A and B are regular languages than C = A $\circ$ B is also regular.

Closure under star: If A is a regular language than C = A* is also a regular language.

