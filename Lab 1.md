# GHDL and GTWave
I downloaded this [Digital System Desgin repository](https://github.com/kevinwlu/dsd) and followed the instuctions in the ghdl folder to download GHDL and GTKWave. 
## Half Adder Example
I used these commands to run the half adder sample code in the repository
```
$ cd dsd
$ cd ghdl
$ ghdl -a ha.vhdl
$ ghdl -a ha_tb.vhdl
$ ghdl -e ha_tb
$ ghdl -r ha_tb --vcd=ha.vcd
ha_tb.vhdl:47:5:@5ns:(assertion error): Reached end of test
$ gtkwave ha.vcd
```
![halfAdder.png]()

## D Flip-flop Example
I used these commands to run the D Flip-flop sample code in the repository
```
$ cd dsd
$ cd ghdl
$ ghdl -a dff.vhdl
$ ghdl -a dff_tb.vhdl
$ ghdl -e dff_tb
$ ghdl -r dff_tb --vcd=dff.vcd
$ gtkwave dff.vcd
```
![DFlipFlop.png]()
