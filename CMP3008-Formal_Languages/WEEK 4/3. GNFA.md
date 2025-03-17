Continuing the abstraction, we can define GNFAs (Generalized NFAs), which uses regex to transition between states.

![[Pasted image 20250310130545.png]]

For convenience, we require that GNFAs always have a special form that meets the following conditions. 
	• The start state has transition arrows going to every other state but no arrows coming in from any other state. 
	• There is only a single accept state, and it has arrows coming in from every other state but no arrows going to any other state. Furthermore, the accept state is not the same as the start state. 
	• Except for the start and accept states, one arrow goes from every state to every other state and also from each state to itself.

