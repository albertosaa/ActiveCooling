## Build instructions

We list below all instructions we followed to build the cooling system for 
a GPU NVIDIA Tesla V100 and for an FPGA Xilinx Alveo U280. The setup can be easily addapted for any card with similar cooling requirements. 

### Air duct desgin and construction 


1. To guarantee mechanical stability and avoid
vibrations, the fan must be fixed at the computer case, and never at the card. To
this end, it is important to employ a computer case with a transverse bracket 
for fans as that one depicted below, which correspons to a locally sourced (Brazil) Nilko NK211 4U
rack-mounting PC case.  

<p align="center">
<img src="../img/nilko.jpg" alt="Computer case" width="50%" /> 
<br>
Fig.1 Nilko NK211 PC case (empty) used in this build.
</p>

<p align="center">
<img src="../img/nilko2.jpg" alt="Computer case" width="50%" />  <br>
Fig.2 Nilko NK211 case with an nVidia Tesla V100 GPU  and all PC components installed. <br> Notice
the 60x60mm cooling fan mounting position (in front of the GPU card).
</p>



2. With the help of a cardboard sheet, for instance, draw the fan opening, mounting holes, and the reference marks for the 
card’s air intake, see below.

<p align="center">
<img src="../img/draw1.jpg" alt="Computer case" width="25%" /> 
<img src="../img/draw2.jpg" alt="Computer case" width="25%" /> 
<br>
Fig.3 Drawing guide lines (left) and full contour (right) of the GPU air intake on the cardboard.
template
</p>

3. Mark the center of each one of the duct openings and measure the vertical and horizontal distances
between them. Such distances will be very important to align the openings when making the 3D model, as
most 3D modeling softwares (we used Autodesk Fusion 360) have center-referenced primitives
(rectangles and circles).

<p align="center">
<img src="../img/draw3.jpg" alt="Computer case" width="25%" /> 
<br>
Fig.4 Cleaned-up outlines of the air duct intake (red) and outlet (blue) <br> and center-to-center
measurements (“x” and “y”).
</p>


4. Use a 3D modeling software to draw a 4mm thick mounting flange for the air duct inlet (similar to
the mounting structure of the fan itself). Draw an hollow frame corresponding to the GPU (or
FPGA) card’s air intake outline on the same diagram, at a plane offset from the origin by the distance
between the fan mounting position and the card’s air intake (when installed on the PC case). Make
this frame 15mm high, 2.5mm thick and oversized in such a way that allow a gap of at least 5mm
between the frame (which will become the duct’s air exit) and the board’s air intake. Refer to the
measurements token on the previous steps to align the two drawings. If possible, use the automatic composing features of the 3D modeling software to draw the air duct’s
body between the two ends (we used the “loft” tool on Autodesk Fusion 360. As this tool deals only
with solid object, we used it twice: for the outer and inner duct shells and subtracted the resulting
objects to obtain an hollow body).

