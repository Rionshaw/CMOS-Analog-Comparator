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
  <li><strong>V+</strong> => Input Signal</li>
  <li><strong>V−</strong> => Reference Voltage</li>
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

<img src="https://github.com/Rionshaw/CMOS-Analog-Comparator/blob/111ed62e52891c44fa58082f10e7f3bf4374a3d8/Screenshot-6.png" alt="Schematic of Analog Comparetor">


<h2>Simulation Results</h2>

<h3>1. DC Sweep Analysis</h3>

<p>
DC sweep analysis was performed to observe comparator switching behavior 
and determine the threshold region where output transition occurs.
</p>

<ul>
  <li>Input voltage swept across operating range.</li>
  <li>Reference voltage maintained at constant value.</li>
  <li>Output transition verified near switching threshold.</li>
</ul>

<img src="https://github.com/Rionshaw/CMOS-Analog-Comparator/blob/111ed62e52891c44fa58082f10e7f3bf4374a3d8/Screenshot-8.png" alt="DC Sweep">

<br>

<h3>2. Transient Analysis</h3>

<p>
Transient simulation was performed to verify dynamic comparator operation 
under time-varying input conditions.
</p>

<ul>
  <li>Sinusoidal input applied to comparator input.</li>
  <li>Reference voltage kept constant.</li>
  <li>Output response monitored over simulation time.</li>
</ul>

<img src="https://github.com/Rionshaw/CMOS-Analog-Comparator/blob/111ed62e52891c44fa58082f10e7f3bf4374a3d8/Screenshot-2.png" alt="Transient Response">

<br>

<h3>3. Propagation Delay Measurement</h3>

<p>
Propagation delay was measured between input threshold crossing 
and corresponding output transition.
</p>

<ul>
  <li>Input crossing point identified.</li>
  <li>Output switching instant measured.</li>
  <li>Time difference calculated as propagation delay.</li>
</ul>

<img src="https://github.com/Rionshaw/CMOS-Analog-Comparator/blob/111ed62e52891c44fa58082f10e7f3bf4374a3d8/Screenshot-4.png" alt="Propagation Delay">
<p>
<strong>Measured Delay =></strong> 36.39 µs
</p>

<br>

<h3>4. Power Consumption Analysis</h3>

<p>
Power consumption was calculated using average supply current 
measured during transient simulation.
</p>

<ul>
  <li>Supply current extracted from VDD source.</li>
  <li>Average current computed using waveform calculator.</li>
  <li>Total power estimated using supply voltage.</li>
</ul>
<img src="https://github.com/Rionshaw/CMOS-Analog-Comparator/blob/111ed62e52891c44fa58082f10e7f3bf4374a3d8/Screenshot-3.png" alt="Power Consumption">
<p>Average Power Calculation</p>
<img src="https://github.com/Rionshaw/CMOS-Analog-Comparator/blob/111ed62e52891c44fa58082f10e7f3bf4374a3d8/Screenshot.png" alt="Average Power">
<p>
<strong>Average Power =></strong> 98.18 µW
</p>

<br>

<h3>5. Performance Summary</h3>

<table>
  <tr>
    <th>Parameter</th>
    <th>Result</th>
  </tr>
  <tr>
    <td>Supply Voltage</td>
    <td>1 V</td>
  </tr>
  <tr>
    <td>Propagation Delay</td>
    <td>36.39 µs</td>
  </tr>
  <tr>
    <td>Average Power</td>
    <td>98.18 µW</td>
  </tr>
</table>
