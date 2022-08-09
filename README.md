<p align="center">
<img src="img/oshwa.png" alt="OSWA Logo" width="20%" /> 
</p>

## Open-source active cooling system for GPU and FPGA accelerator cards 

An open-source, Arduino-based, programmable active cooling system for a
GPU NVIDIA Tesla V100 and for a FGPA Xilinx Alveo U280 cards installed
in standard computer cases.

<img src="img/tesla.jpg" alt="drawing" width="49%"/> <img src="img/xl.jpg" alt="drawing" width="49%"/>

### Overview 

Typically, high-performance Graphics Processing Units (GPU) and Field
Programmable Gate Arrays (FPGA) accelerators are high-power demanding
elements, designed to be mounted in specialized, high-cost, racks with intense
forced airflow systems to assure their functioning within proper thermal
limits. We present here an open-source, Arduino-based, programmable
active cooling system for GPU and FPGA cards that allow their
installation in common computer cases. Only standard components and
simple 3D-printed pieces are employed in our design. We built and have
been continuously using this cooling system for a GPU NVIDIA Tesla V100
and an FPGA Xilinx Alveo U280, both mounted
in   common PCIe motherboards (ASUS PRIME Intel H510M-E), installed in a
standard rack-mounted computer case  and operating in an air-conditioned datacenter. The setup is inexpensive and has proved
to be flexible and extremely reliable. Furthermore, it can be easily
adapted for any other card or element requiring similar cooling.

For the rationale and overall description of the project, see the accompanying
[paper](cooling-paper.pdf). For the full build instructions, see the [hardware
details](hardware/). For the Arduino programming and electronics, see the
[controller details](https://github.com/RodLophus/ArduinoFanController).

### License 

The hardware presented here is freely available under a
[CERN-OHL-S-2.0](https://spdx.org/licenses/CERN-OHL-S-2.0.html) license, which can be also found [here](HWLICENSE.md).

The software and documentation are freely available under an [MIT
license](https://opensource.org/licenses/MIT), which can be also found 
[here](LICENSE).

### Contact 

This project was carried out in the Institute of Mathematics,
Statistics, and Scientific Computing of the University of Campinas, SP,
Brazil. For further questions, please contact the developer Rodolfo Manin
(<rodolfo@ime.unicamp.br>) or the Principal Investigator Alberto Saa
(<asaa@ime.unicamp.br>).

### Citation 

R. Manin and A. Saa, Open-source active cooling system for GPU and FPGA
accelerator cards (2002).

### Funding 

The work of A. Saa is supported by CNPq (grant 302674/2018-7) and FAPESP
(grant 21/09293-7).

### Dataset Metadata 

<div itemscope itemtype="http://schema.org/Dataset">
<table>
<tr>
<th>property</th>
<th>value</th>
</tr>
<tr>
<td>name</td>
<td><code itemprop="name">Open-source active cooling system for GPU and FPGA accelerator cards</code></td>
</tr>
<tr>
<td>description</td>
<td><code itemprop="description"> We present here an open-source, Arduino-based, programmable active cooling system for GPU and FPGA cards that allow their installation in common computer cases. Only standard components and simple 3D-printed pieces are employed in our design. We built and have been continuously using this cooling system for a GPU NVIDIA Tesla V100 and an FPGA Xilinx Alveo U280. The setup is inexpensive and has proved to be flexible and extremely reliable. Furthermore, it can be easily adapted for any other card or element requiring similar cooling. </code></td>
</tr>
</tr>
<tr>
<td>url</td>
<td><code itemprop="url">https://github.com/albertosaa/ActiveCooling</code></td>
</tr>
<tr>
<td>sameAs</td>
<td><code itemprop="sameAs">https://github.com/albertosaa/ActiveCooling</code></td>
</tr>
<tr>
<td>citation</td>
<td><code itemprop="citation"> R. Manin and A. Saa, Open-source active cooling system for GPU and FPGA accelerator cards (2002).  </code></td>
</tr>
<tr>
<td>hw license</td>
<td>
<div itemscope itemtype="http://schema.org/CreativeWork" itemprop="license">
<table>
<tr>
<th>property</th>
<th>value</th>
</tr>
<tr>
<td>name</td>
<td><code itemprop="name">CERN-OHL-S-2.0</code></td>
</tr>
<tr>
<td>url</td>
<td><code itemprop="url">https://spdx.org/licenses/CERN-OHL-S-2.0.html</code></td>
</tr>
</table>
</div>
</td>
</tr>
<tr>
<td>sw license</td>
<td>
<div itemscope itemtype="http://schema.org/CreativeWork" itemprop="license">
<table>
<tr>
<th>property</th>
<th>value</th>
</tr>
<tr>
<td>name</td>
<td><code itemprop="name">MIT</code></td>
</tr>
<tr>
<td>url</td>
<td><code itemprop="url">https://opensource.org/licenses/MIT</code></td>
</tr>
</table>
</div>
</td>
</tr>
<tr>
<td>docs license</td>
<td>
<div itemscope itemtype="http://schema.org/CreativeWork" itemprop="license">
<table>
<tr>
<th>property</th>
<th>value</th>
</tr>
<tr>
<td>name</td>
<td><code itemprop="name">MIT</code></td>
</tr>
<tr>
<td>url</td>
<td><code itemprop="url">https://opensource.org/licenses/MIT</code></td>
</tr>
</table>
</div>
</td>
</tr>
<tr>
</table>
</div>
</td>
</tr>
</table>
</div>
