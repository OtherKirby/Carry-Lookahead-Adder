# Carry Lookahead Adder (CLA)
A simulation file of a fast 4 bit adder, with half adder, and CLA logic block.

## How to open
1. Download Logisim from SourceForge: https://sourceforge.net/projects/circuit/
2. Save this .circ file to a folder on your computer.
3. Under **File** in Logisim, click **Open** and find the path to the .circ file and open it.

## Roadmap
- [x] Fix Carry In on main circuit.
- [ ] Implement 7 segment decimal display for easier I/O reading
- [ ] Edit circuit appearance to match general CLA shape.
- [ ] Explain steps more thoroughly in the .circ file
- [ ] Label gates, I/O more effectively.
- [ ] Upload image of finished schematic for quick reference.


## Steps to implement a CLA
1. Follow the formula C(i+1) = G(i) + (P(i) + C(i)); where C is the carry bit, G is the generate, and P is the propogate.
2. Substitute this formula in for the same number of times as the amount of bits you will be adding.
_-(4 bit CLA will have a logic block with 4 outputs, C1, C3, C4.)
-(NO C0 because that would call for i = -1, which is impossible)_
3. Substitute the previous C value in each formula.
_- (Substitute C1 into C2, C2 into C3, etc...)_

## Other Comments
- See the [Wikipedia Page](https://en.wikipedia.org/wiki/Carry-lookahead_adder) for more information on this adder.
- I found it easier to implement my CLA using **individual** I/O bits rather than a multibit I/O for the 
sake of demonstration
