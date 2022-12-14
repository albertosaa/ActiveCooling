<p align="center">
<img src="../img/oshwa.png" alt="OSWA Logo" width="20%" /> 
</p>

# Build instructions

We describe below all steps we have followed to build the cooling system for a GPU NVIDIA Tesla V100 and an FPGA Xilinx Alveo U280. The setup can be easily adapted for any card with similar cooling requirements. 

## Air duct desgin and construction 

### Requires

* 3D printer
* High-temperature PLA filament for the final ducts
* Optional: Regular PLA filament for the test-fit
* Cardboard sheets 

### Instructions

1. To guarantee mechanical stability and avoid vibrations, the fan must be fixed in the computer case, and never at the card. To this end, it is important to employ a computer case with a transverse bracket for fans like that one depicted below, which corresponds to a locally sourced (Brazil) Nilko NK211 4U rack-mounting PC case.

<p align="center">
<img src="../img/nilko.jpg"   width="50%" /> 
<br>
Fig.1 An empty Nilko NK211 PC case used in this build.  Notice the transverse bracket for fans.
</p>

<p align="center">
<img src="../img/nilko2.jpg"   width="50%" />  <br>
Fig.2 Nilko NK211 case with the GPU nVidia Tesla V100  and all PC components installed. <br> Notice
the 60x60x38 mm cooling fan mounting position (in front of the GPU card).
</p>



2. With the help of a cardboard sheet, for instance, draw the fan opening, mounting holes, and the reference marks for the 
card’s air intake, see below.

<p align="center">
<img src="../img/draw1.jpg"  width="25%" /> 
<img src="../img/draw2.jpg"   width="25%" /> 
<br>
Fig.3 Drawing guide lines (left) and full contour (right) of the GPU air intake on the cardboard.
template
</p>

3. Mark the center of the duct openings and measure the vertical and horizontal distances between them. Such distances will be very important to align the openings when making the 3D model, as most 3D modeling software (we used Autodesk Fusion 360) have center-referenced primitives (rectangles and circles).

<p align="center">
<img src="../img/draw3.jpg"   width="25%" /> 
<br>
Fig.4 Cleaned-up outlines of the air duct intake (red) and outlet (blue) <br> and the respective center-to-center
measurements (“x” and “y”).
</p>


4. By using some 3D modeling software, draw a 4mm thick mounting flange for the air duct inlet (similar to the fan mounting structure). Draw a hollow frame corresponding to the GPU (or FPGA) card’s air intake outline on the same diagram, at a plane with an offset from the origin given by the distance
between the fan mounting position and the card’s air intake (when installed in the PC case). Make this frame 15 mm high, 2.5 mm thick, and oversized in such a way that allows a gap of at least 5mm between the frame (which will become the duct’s air exit) and the board’s air intake. Refer to the measurements taken in the previous steps to align the two drawings. If possible, use the automatic composing features of the 3D modeling software to draw the air duct’s body between the two ends (we used the “loft” tool on Autodesk Fusion 360. As this tool deals only with a solid object, we used it twice: for the outer and inner duct shells and subtracted the resulting objects to obtain a hollow body).

<p align="center">
<img src="../img/3DP.png"   width="25%" /> 
<img src="../img/3DP2.png"   width="25%" /> 
<br>
Fig.5 Modeling the ends of the air duct (left) and using the 3D modeling software tools <br> to automatically
generate the complete smooth structure connecting them (right).
</p>

5. Make a test-fit part of the complete air duct using a 3D printer. You can use regular PLA and low
filling (about 10%) for this test-fit. Mount the test-fit part on the PC case and measure the gap between
the duct and the CPU (of FPGA) card. Modify the 3D model in order to make this gap 4mm wide
and uniform on all sides.

<p align="center">
<img src="../img/nvidiatest.jpg"   width="50%" />  <br>
Fig.6 Test-fit piece mounted on the PC case. Notice the wide gap <br> between the duct
and the nVidia GPU card’s air intake.
</p>

6. Make the final air duct using the 3D printer. Use High-Temperature PLA (also called “Premium PLA”) or similar material, as most regular PLAs soften and get deformed at temperatures as low as 50°C, and a higher filling rate (we used 80%). The figure below depicts the ducts for our cards. For sake of illustration, we attach the respective 3D Manufacturing Format files (.3mf and .f3d), but of course, the design must be customized for the particular card  and computer case in question.

<p align="center">
<img src="../img/duct1.jpg"   width="30%" /> 
<img src="../img/duct1.jpg"   width="30%" /> 
<br>
Fig.7 Final   air ducts for the nVidia Tesla V100 GPU (left) and Xilinx Alveo
U280 FPGA cards (right) for our computer case.
</p>

## Assembly Instructions

### Requires

* 3D-printed ducts
* [Arduino-based controller](https://github.com/RodLophus/ArduinoFanController)
* 60x60x38mm 4-pin cooler fan with pulse width modulation (PWM). Examples: [Sanyo Denki model 9GA0612P1K611](https://products.sanyodenki.com/en/sanace/dc/dc-fan/9GA0612P1K60), [Delta Electronics model PFC0612DE](https://www.delta-fan.com/Download/Spec/PFC0612DE-F00.pdf)

<p align="center">
<img src="../img/fan.jpg"  width="20%" /> 
</p>

* Adhesive EPDM foam 6mmx10mm tape

<p align="center">
<img src="../img/tape.jpg"   width="20%" /> 
</p>

* M4x12mm allen bolts with nuts, regular washers and lock washers

<p align="center">
<img src="../img/bolts.jpg"   width="20%" /> 
</p>

### Instructions 

1. Apply the adhesive foam  on the internal wall of the air duct outlet
to seal the gap between the duct and the card.

<p align="center">
<img src="../img/ass1.jpg"   width="50%" /> 
<br>
Fig.8 Final air duct with the rubber foam applied.
</p>

2. Install the cooler fan and the air duct on the PC case’s traverse bracket.  Use M4x12mm allen bolts, nuts, and lock washers to prevent losing due to the vibration.

<p align="center">
<img src="../img/ass2.jpg"   width="70%" /> 
<br>
Fig.9 Air duct and fan mounted on the PC case’s bracket.
</p>

3.  To prevent the rubber foam from being dragged, use some paper sheets to insert the card's body into the 
duct outlet. Look into the air duct through the fan and check if the power cable for the high performance card
is in place (along the duct’s side). Use a long screwdriver to set the cable in place if needed.

<p align="center">
<img src="../img/teslapaper.jpg"   width="70%" /> 
<br>
Fig.10 Positioning and installing the cooling system into the PC case.
</p>

4. Secure all cables and wires inside the PC case using cable ties or other cable management system.
Make sure no cable is in the way of the air flow neither can came in contact with the fan blades.

<p align="center">
<img src="../img/tesla.jpg"   width="35%" /> 
<img src="../img/xl.jpg"   width="35%" /> 
<br>

5. Install the fan controller and connect the high performance card’s fan to one of its temperature-
controlled PWM outputs. Install the controller’s temperature sensor on the back of the case, in the
board’s hot air outlet. Extend the sensor’s wires if needed.

<p align="center">
<img src="../img/ass4.jpg"  width="35%" /> 
<img src="../img/ass5.jpg"  width="35%" /> 
<br>
  
6. Use some burn-in test program to stress the high performance card (for example, [gpu-burn](https://github.com/wilicc/gpu-burn) for the
nVidia Tesla). Configure the temperature controller to ensure
the board works within thermal specifications even with maximum power dissipation. We have set
the fan power (PWM duty cycle) at 40% and 100%, respectively for temperatures below 40°C and
above 55°C (for the intermediate temperatures, the fan power is linearly increased). This was done
on the Arduino-based fan controller using the settings shown below:
  
<p align="center">
<img src="../img/arduinocontrol.png"  width="75%" /> 
<br>

7. With this setup we saw a maximum GPU temperature of 67°C for a power draw of about 230W (as
reported by nVidia’s “nvidia-smi” utility) when running gpu-burn for 15 minutes. The ambient
temperature was 23°C.
  
<p align="center">
<img src="../img/burn.png"   width="75%" /> 
<br>
  
