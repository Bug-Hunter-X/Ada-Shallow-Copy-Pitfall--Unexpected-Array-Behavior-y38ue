# Ada Shallow Copy Pitfall

This example highlights a common misunderstanding in Ada regarding array assignment.  The code demonstrates that when an array is assigned to another array (`B := A`), a shallow copy is performed.  This means that both arrays initially point to the same memory location. Consequently, modifications to one array will *not* affect the other.  This behavior may differ from some other languages where deep copying is the default. 

The provided solution demonstrates a way to make a deep copy to address the problem.

**Relevant Ada Concepts:**
* Array assignment
* Shallow copy vs. Deep copy
* Array aggregates
* Iteration
