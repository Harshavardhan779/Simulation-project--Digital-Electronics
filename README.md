# TITTLE
Design and simulate the logic diagram using Verilog.
F=(X+Y')(X'+Y)Z'
# THEORY
Product Of Sum:

i.) POS stands for Product of Sums.

ii.) It is a technique of defining boolean terms as a product of sum terms.

iii.) It prefers maxterms.

iv.) In the case of POS, the Maxterms are defined as ‘M’

v.) It gives LOW(0) output.

vi.) In POS, we can get the final term by multiplying the sum terms.

K-Map:

A Karnaugh map (K-map) is a visual method used to simplify the algebraic expressions in Boolean functions without having to resort to complex theorems or equation manipulations. A K-map can be thought of as a special version of a truth table that makes it easier to map out parameter values and arrive at a simplified Boolean expression.
# LOGIC DIAGRAM
![OUTPUT](/de%20sa2-1.png)
# NETLIST DIAGRAM
![OUTPUT](/de%20sa2-2.png)

# TIMING DIAGRAM
![OUTPUT](/de%20sa2-3.png)

# PROGRAM
```python
/* 
Name:Harshavardhan
Reg No:212222240114
*/
module assignment1 (x,y,z,f);
input x,y,z;
output f;
wire a,b,c,d,e;
not (a,x);
not (b,y);
not (c,z);
and (d,a,b,c);
and (e,x,y,c);
or (f,d,e);
endmodule
```
# REFERENCE
https://www.javatpoint.com/number-system-in-digital-electronics