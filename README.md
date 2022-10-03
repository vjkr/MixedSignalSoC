# MixedSignalSoC
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

