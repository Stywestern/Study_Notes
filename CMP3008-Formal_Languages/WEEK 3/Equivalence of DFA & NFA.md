A language is accepted by the eqDFA iff it is also accepted bu eqNFA, which makes sense as it is more lax.
To construct the DFA from the NFA, the DFA should contain all of the possible states conjured by NFA. If NFA has 3 states, the DFA will at least have 8 (2^3). 
![[Pasted image 20250224140359.png]]

Then we select appropriate start and accept states.

You may also trim the states if you deem them unreachable, like here:
![[Pasted image 20250224140721.png]]

There were no arrows going to {1,2} and and {1}, so they are irrelevant. 