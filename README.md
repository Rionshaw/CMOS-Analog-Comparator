<h1>CMOS Analog Comparator Design using gpdk090</h1>


<p>
This project presents the transistor-level design and simulation of a CMOS Analog Comparator 
implemented using the <strong>gpdk090 CMOS technology library</strong> in 
<strong>Cadence Virtuoso</strong>. The comparator compares two analog voltages and produces 
a digital output depending on which input signal is larger.
</p>

<h3>Design Features</h3>

<ul>
  <li>Differential NMOS input pair</li>
  <li>PMOS active load</li>
  <li>Tail current biasing</li>
  <li>Gain stage</li>
  <li>CMOS output stage</li>
</ul>

<p>
The project demonstrates the analog IC design flow in <strong>Cadence Virtuoso</strong>, 
including schematic implementation, transient analysis, DC sweep characterization, 
propagation delay measurement, and power calculation.
</p>


<h2>Comparator Operation</h2>

<p>
The comparator evaluates two input voltages and generates a digital output based on their relative magnitude.
</p>

<ul>
  <li><strong>V+</strong> : Input Signal</li>
  <li><strong>V−</strong> : Reference Voltage</li>
</ul>

<h3>Logic Behavior</h3>

<table>
  <tr>
    <th>Condition</th>
    <th>Output</th>
  </tr>
  <tr>
    <td>V+ &gt; V−</td>
    <td>HIGH</td>
  </tr>
  <tr>
    <td>V+ &lt; V−</td>
    <td>LOW</td>
  </tr>
</table>

<br>

<h2>Circuit Architecture</h2>

<p>
The CMOS Analog Comparator is implemented using a multi-stage analog architecture for signal comparison and amplification.
</p>

<pre>
Differential Pair
        ↓
Active Load
        ↓
Gain Stage
        ↓
CMOS Output Stage
</pre>


<h2>Objective</h2>

<ul>
  <li>Design CMOS Analog Comparator using GPDK090 technology.</li>
  <li>Compare analog inputs to produce digital output.</li>
  <li>Analyze DC and transient response characteristics.</li>
  <li>Evaluate propagation delay and power consumption.</li>
</ul>

<br>

<h2>Tools Used</h2>

<ul>
  <li>Cadence Virtuoso</li>
  <li>GPDK090 CMOS Technology Library</li>
  <li>Analog Design Environment (ADE)</li>
  <li>Waveform Viewer</li>
</ul>



<h2>Schematic Design</h2>

<img src="https://github.com/Rionshaw/cmos-nand-gate-gpdk090/blob/0c17e513281cb6642c11c4d4fa045b23dae0888b/Screenshot-4.png" alt="Schematic of NAND gate">
