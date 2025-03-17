Unlike DFAs, the state after the operation is not determined as any one state. e.g.
![[Pasted image 20250224132330.png]]
3 main differences with DFAs:
	Here q1 can go to q2 or q0 given the same input like 0. 
	There exist a $\lambda$ operation that transitions q0 to q2 without any input.
	And also there are undefined operations like op(q2, 0) = ?

The conditions for acceptance change here, as a string (like 10) can either go to an accepted state or not. We accept all strings where
$\delta$* (q0, s) = F, meaning if there is any possibility we accept it.

As for substring acceptance, the same rules apply. From any state see if there is a possibility of acceptance.

