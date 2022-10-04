# Introduction to Skywater and PDKs
## TIm Edwards
Efabless provides a harness chip for shuttle program where a RISCV processor is provided with remaining space for use. Wire bumps are also made available. Hence die gets auto connected to external world. Bumps are done for 'redistribution layers' often done by specialized parties.
![image](https://user-images.githubusercontent.com/16399079/193616251-c0be498b-2838-4b97-9d7f-61f1708277f5.png)
Skywater works with most commericail tools but may not complete the requirements because of incompatibility and legal issues.
Hence Skywater is best suited for opensource works.
![image](https://user-images.githubusercontent.com/16399079/193616964-3178e4f9-6a06-4c5f-a1aa-73eb9c9b7803.png)
![image](https://user-images.githubusercontent.com/16399079/193618238-014ee07e-b727-4a1f-b37b-41fdfb4db968.png)
Above images show the open source EDA tools supported by Open_pdk
https://skywater-pdk.readthedocs.io/en/main/contents/libraries/foundry-provided.html
tells naming of skywater libraries. Example
 sky130_fd_sc_hs (high speed), sky130_fd_sc_ms (medium speed), where fd is foundry and sc is stanard cell
Major types are
![image](https://user-images.githubusercontent.com/16399079/193619684-d24d89cf-0683-415b-a515-853b9d11d16a.png)

Below is the filestructure. A in sky130A indicates a variant. for simplicity single letter A can be 1,2,3,...
![image](https://user-images.githubusercontent.com/16399079/193620363-c6ae61d3-63b4-427c-81f9-0772c42827be.png)
Designing NPN on die
![image](https://user-images.githubusercontent.com/16399079/193623473-fc0d6d10-1363-4111-9eb0-e3f43937d622.png)
Resistors can be designed by poly or diffusions. poly is the best choice. Discrete widths are available for usage. So resitances are to be careflly calculated.  Certain ready made FETs are made available as GDS files which designers should use as is.
![image](https://user-images.githubusercontent.com/16399079/193625354-4458178b-4117-42a2-b7b6-1c04acdd2195.png)

# Intro toMixed Signal design
## Sumanto KAur

Transducers convert physical signals to electrical
![image](https://user-images.githubusercontent.com/16399079/193729506-2c711407-5999-499b-a765-4bed29178401.png)
Analog Signl vs Digitl signal
 Mixed mode design in esim
 tools used are
 1. eSim created by FOSSEE IIT B
 2. MakerChip which is browser IDE for verilog
 3. NGSPICE + VERILATOR = NGVERI    --> Analog + Digital = Mixed

# Handson esim
lab instance is on 
![image](https://user-images.githubusercontent.com/16399079/193731973-cff15255-9e2f-473f-a5f5-7fb3940bb5bb.png)

install from here
![image](https://user-images.githubusercontent.com/16399079/193731193-c143199e-028b-4834-b4ea-4a5154e8b299.png)
run sh file for installing
in lab instance esim is already installed. open terminal anywhere and launch tool by typing esim
see makerchip ngveri
![image](https://user-images.githubusercontent.com/16399079/193731863-a38e0536-0a24-48d5-95ae-209cbf5e1620.png)
aFTER removing lint errors and observing tlv file which has random numbers tested. results below
![image](https://user-images.githubusercontent.com/16399079/193735567-2509c64c-bf35-4261-ad4a-10c8b4cb4574.png)
also got results for counter
![image](https://user-images.githubusercontent.com/16399079/193785019-86b0b097-5341-4d3d-92b3-635a1b072784.png)

verilog to ngspice conversion successful. Not sure where the file is!
![image](https://user-images.githubusercontent.com/16399079/193788127-83f2ce65-cac3-4ab3-bb0a-8f0d82221427.png)
completed drawing this on schematic using our own counter!!
![image](https://user-images.githubusercontent.com/16399079/193797951-2fbf341b-0100-480c-b7e0-620fbb155b4c.png)



