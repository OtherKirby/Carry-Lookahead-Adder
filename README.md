# Carry Lookahead Adder (CLA)
A simulation file of a fast 4 bit adder, with half adder, and CLA logic block.

## How to open
1. Download Logisim from SourceForge: https://sourceforge.net/projects/circuit/
2. Save this .circ file to a folder on your computer.
3. Under **File** in Logisim, click **Open** and find the path to the .circ file and open it.

## Roadmap
- **[ ] Fix arithmetic inconsistencies on main circuit.**
- [ ] Edit circuit appearance to match general CLA shape.
- [ ] Explain steps more thoroughly in the .circ file
- [ ] Label gates, I/O more effectively.
- [ ] Upload image of finished schematic for quick reference.<br/>
~~- [ ] Implement 7 segment decimal display for easier I/O reading~~


## Steps to implement a CLA
1. Follow the formula **C<sub>i+1</sub> = G<sub>i</sub> + (P<sub>i</sub> + C<sub>i</sub>)**; where C is the carry bit, G is the generate, and P is the propogate.
2. Substitute this formula in for the same number of times as the amount of bits you will be adding.<br/>
_-(4 bit CLA will have a logic block with 4 outputs, C<sub>1</sub>, C<sub>2</sub> C<sub>3</sub>, C<sub>4</sub>.)<br/>
-(NO C<sub>0</sub> because that would call for i = -1, which is impossible)_
3. Substitute the previous C value in each formula.<br/>
_- (Substitute C<sub>1</sub> into C<sub>2</sub>, C<sub>2</sub> into C<sub>3</sub>, etc...)_

## Other Comments
- See the [Wikipedia Page](https://en.wikipedia.org/wiki/Carry-lookahead_adder) for more information on this adder.
- I found it easier to implement my CLA using **individual** I/O bits rather than a multibit I/O for the 
sake of demonstration
