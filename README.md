# 🧠 Digital VLSI SoC Design and Planning

> 📚 Documentation of my learning journey through this course on **Digital VLSI System-on-Chip (SoC) Design and Planning**.

---

<details>
  <summary><strong>📘 Day-wise Digital VLSI SoC Design Journey (Click to Expand)</strong></summary>

  <ul>
    <li>
      <a href="#📅-day-1-–-openlane--synthesis-flow">
        📅 Day 1 – Open-source EDA, OpenLANE & RTL-to-GDS Overview
      </a>
    </li>
    <li>
      <a href="#📅-day-2-–-floorplanning-power-planning--placement">
        📅 Day 2 – Floorplanning, Placement & Library Characterization
      </a>
    </li>
    <li>
      <a href="#📅-day-3-–-standard-cell-design-layout--characterization">
        📅 Day 3 – Standard Cell Design & SPICE Characterization
      </a>
    </li>
    <li>
      <a href="#📅-day-4-–-timing-analysis--clock-tree-synthesis">
        📅 Day 4 – Timing Analysis & Clock Tree Synthesis
      </a>
    </li>
    <li>
      <a href="#📅-day-5-–-final-steps-cts-pdn--routing">
        📅 Day 5 – Routing, DRC & Final RTL-to-GDS Closure
      </a>
    </li>
  </ul>
</details>

---

<details>
  <summary><strong>🖼️ Quick Image Navigator (Jump to Any Image Section)</strong></summary>

  <details>
    <summary><strong>📅 Day 1</strong></summary>
    <ul>
      <li><a href="#day1-lab-part1">Lab Day 1 – Part 1</a></li>
      <li><a href="#day1-lab-part2">Lab Day 1 – Part 2</a></li>
      <li><a href="#day1-lab-part3">Lab Day 1 – Part 3</a></li>
      <li><a href="#day1-lab-part4">Lab Day 1 – Part 4</a></li>
      <li><a href="#day1-lab-part5">Lab Day 1 – Part 5</a></li>
      <li><a href="#day1-lab-part6">Lab Day 1 – Part 6</a></li>
      <li><a href="#day1-lab-part7">Lab Day 1 – Part 7</a></li>
      <li><a href="#day1-lab-part8">Lab Day 1 – Part 8</a></li>
      <li><a href="#day1-openlane-work-dir">OpenLane Work Directory</a></li>
      <li><a href="#day1-openlane-launch">OpenLane Launch</a></li>
      <li><a href="#day1-config-tcl">config.tcl File</a></li>
      <li><a href="#day1-prep-design">Design Preparation – picorv32a</a></li>
      <li><a href="#day1-new-runs">New Runs Directory Created</a></li>
      <li><a href="#day1-results-folder">Results Folder</a></li>
      <li><a href="#day1-success-synth">✅ Successful Synthesis</a></li>
      <li><a href="#day1-ff-count">🔢 Flip-Flop Count: 1613</a></li>
      <li><a href="#day1-ff-ratio-final">📊 FF Ratio (Final)</a></li>
      <li><a href="#day1-ff-ratio-pct">📊 FF Ratio (Percentage)</a></li>
      <li><a href="#day1-netlist-runs">📄 Synthesized Netlist (Runs Folder)</a></li>
      <li><a href="#day1-netlist-gedit">📄 Synthesized Netlist (Gedit View)</a></li>
      <li><a href="#day1-yosys-stats">📈 Yosys Statistics Report</a></li>
      <li><a href="#day1-yosys-stats-gedit">📈 Yosys Stats (Gedit View)</a></li>
      <li><a href="#day1-available-reports">📋 Available Reports</a></li>
      <li><a href="#day1-opensta-timing">⏱️ OpenSTA Timing Report</a></li>
    </ul>
  </details>

  <details>
    <summary><strong>📅 Day 2</strong></summary>
    <ul>
      <li><a href="#day2-decap">Decoupling Capacitors</a></li>
      <li><a href="#day2-decap-example">Decoupling Capacitor – Example</a></li>
      <li><a href="#day2-ground-bounce">Ground Bounce</a></li>
      <li><a href="#day2-voltage-droop">Voltage Droop</a></li>
      <li><a href="#day2-droop-solution">Solution to Voltage Droop</a></li>
      <li><a href="#day2-multi-supply">Multiple Supplies & Grounds</a></li>
      <li><a href="#day2-power-plan">Power Planning & Meshes</a></li>
      <li><a href="#day2-design-to-place">Design to be Placed</a></li>
      <li><a href="#day2-port-placement">Port Placement on Die</a></li>
      <li><a href="#day2-ready-pnr">Ready for PnR</a></li>
      <li><a href="#day2-config-readme">Config README</a></li>
      <li><a href="#day2-core-util">Floorplanning & Core Utilization</a></li>
      <li><a href="#day2-floorplan-tcl">floorplan.tcl Script</a></li>
      <li><a href="#day2-design-config">Design Config Files</a></li>
      <li><a href="#day2-config-in-folder">config.tcl in Design Folder</a></li>
      <li><a href="#day2-success-floorplan">✅ Successful Floorplan</a></li>
      <li><a href="#day2-floorplan-def-png">Floorplan DEF (PNG)</a></li>
      <li><a href="#day2-floorplan-def-gedit">Floorplan DEF (Gedit)</a></li>
      <li><a href="#day2-magic-floorplan">Magic Output – Floorplan</a></li>
      <li><a href="#day2-pin-select">Pin Selection in Magic</a></li>
      <li><a href="#day2-std-cells-pre">Std Cells Visible Pre-Placement</a></li>
      <li><a href="#day2-post-floorplan-magic">Post-Floorplan Magic View</a></li>
      <li><a href="#day2-sta-slide">STA Slide</a></li>
      <li><a href="#day2-success-placement">✅ Successful Placement</a></li>
      <li><a href="#day2-placement-output">Placement Run Output Directory</a></li>
      <li><a href="#day2-picorv32-placement">picorv32 Post-Placement View</a></li>
      <li><a href="#day2-magic-floorplan-tool">Magic – Floorplan (Tool View)</a></li>
      <li><a href="#day2-magic-post-place">Magic – Post Placement</a></li>
      <li><a href="#day2-cell-flow-lecture">Lecture – Cell Design Flow</a></li>
      <li><a href="#day2-cell-flow">Cell Design Flow</a></li>
      <li><a href="#day2-complete-flow">Complete Cell Design Flow</a></li>
      <li><a href="#day2-char-flow">Characterization Flow</a></li>
      <li><a href="#day2-model-file">Model File (.txt)</a></li>
    </ul>
  </details>

  <details>
    <summary><strong>📅 Day 3</strong></summary>
    <ul>
      <li><a href="#day3-magic-inverter">Magic Custom Inverter</a></li>
      <li><a href="#day3-inverter-layout">Inverter Layout View</a></li>
      <li><a href="#day3-cmos-fab">CMOS Fabrication Process Overview</a></li>
      <li><a href="#day3-nmos">NMOS Transistor Identified</a></li>
      <li><a href="#day3-pmos">PMOS Transistor Identified</a></li>
      <li><a href="#day3-output-y">Output Y Connected to PMOS & NMOS Drains</a></li>
      <li><a href="#day3-pmos-vdd">PMOS Source → VDD</a></li>
      <li><a href="#day3-nmos-vss">NMOS Source → VSS</a></li>
      <li><a href="#day3-drc-error">Deleting Layout to Trigger DRC Error</a></li>
      <li><a href="#day3-drc-understand">Selecting Random Area to Understand DRC</a></li>
      <li><a href="#day3-via-view">Via View in Magic</a></li>
      <li><a href="#day3-load-poly">Load Poly Layer in Magic</a></li>
      <li><a href="#day3-spice-cmd">SPICE Extraction Commands</a></li>
      <li><a href="#day3-spice-file">Generated SPICE Netlist</a></li>
      <li><a href="#day3-spice-explain">SPICE File Explanation</a></li>
      <li><a href="#day3-grid-meas">Grid Measurement</a></li>
      <li><a href="#day3-spice-v1">Updated SPICE File – Version 1</a></li>
      <li><a href="#day3-spice-v2">Updated SPICE File – Version 2</a></li>
      <li><a href="#day3-ngspice-run">Ngspice Simulation Run</a></li>
      <li><a href="#day3-waveform">Ngspice Waveform – Inverter</a></li>
      <li><a href="#day3-rise-20">Rise Time – 20% Point</a></li>
      <li><a href="#day3-x-066y">X Value at 0.66·Y</a></li>
      <li><a href="#day3-rise-80">Rise Time – 80% Point</a></li>
      <li><a href="#day3-x-264y">X Value at 2.64·Y</a></li>
      <li><a href="#day3-skywater-cmd">Commands to Download Corrupted SkyWater Tech File</a></li>
      <li><a href="#day3-met3-files">Metal 3 (M3) Magic Files</a></li>
      <li><a href="#day3-met3-layout">Metal 3 Layout View</a></li>
      <li><a href="#day3-tech-v1">Edited Tech File – Version 1</a></li>
      <li><a href="#day3-tech-v2">Edited Tech File – Version 2</a></li>
      <li><a href="#day3-updated-drc">Updated DRC After Fix</a></li>
    </ul>
  </details>

  <details>
    <summary><strong>📅 Day 4</strong></summary>
    <ul>
      <li><a href="#day4-tracks">Tracks Info File</a></li>
      <li><a href="#day4-lef-ss">LEF File (Slow-Slow Corner)</a></li>
      <li><a href="#day4-copy-lef">Commands to Copy LEF File</a></li>
      <li><a href="#day4-include-lef">Commands to Include New LEF</a></li>
      <li><a href="#day4-mod-config">Modified config.tcl</a></li>
      <li><a href="#day4-prep-final">Prep Final Design</a></li>
      <li><a href="#day4-synth1">✅ Successful Synthesis (Initial)</a></li>
      <li><a href="#day4-synth2">✅ Successful Synthesis – Second Run</a></li>
      <li><a href="#day4-optimized-synth">✅ Optimized Synthesis Completed</a></li>
      <li><a href="#day4-save1">💾 Save Checkpoint #1</a></li>
      <li><a href="#day4-fail-floorplan">❌ Failed Initial Floorplan</a></li>
      <li><a href="#day4-manual-floorplan">✅ Manual Multi-Step Floorplan</a></li>
      <li><a href="#day4-placement-done">✅ Placement Completed</a></li>
      <li><a href="#day4-placement-def">Placement DEF File</a></li>
      <li><a href="#day4-custom-cell">Instance of Our Custom Cell</a></li>
      <li><a href="#day4-expanded-view">Expanded View of Custom Cell</a></li>
      <li><a href="#day4-base-sdc">Base SDC Constraints File</a></li>
      <li><a href="#day4-pre-sta">Pre-STA Configuration</a></li>
      <li><a href="#day4-sta1">STA Run – Initial</a></li>
      <li><a href="#day4-sta2">STA Run – Second Pass</a></li>
      <li><a href="#day4-sta-final">STA – Final Verification</a></li>
      <li><a href="#day4-cond1">✅ Condition 1 Verified</a></li>
      <li><a href="#day4-cond2">✅ Condition 2 Verified</a></li>
      <li><a href="#day4-cond3">Condition 3 (Under Evaluation)</a></li>
      <li><a href="#day4-or-fanout">OR Gate with Multiple Fanouts</a></li>
      <li><a href="#day4-cell-opt">Cell Optimization Applied</a></li>
      <li><a href="#day4-eco">✅ Basic ECO Complete</a></li>
    </ul>
  </details>

  <details>
    <summary><strong>📅 Day 5</strong></summary>
    <ul>
      <li><a href="#day5-final-place">Final Placement View</a></li>
      <li><a href="#day5-final-opt">Final Optimizations Applied</a></li>
      <li><a href="#day5-cts">✅ Final Successful CTS</a></li>
      <li><a href="#day5-pdn">Final PDN Implementation</a></li>
      <li><a href="#day5-pdn-def">PDN in DEF Format</a></li>
      <li><a href="#day5-pdn-lines1">PDN Power Lines – View 1</a></li>
      <li><a href="#day5-pdn-lines2">PDN Power Lines – View 2</a></li>
      <li><a href="#day5-routing-ongoing">Routing in Progress</a></li>
      <li><a href="#day5-routing-done">✅ Routing Completed</a></li>
      <li><a href="#day5-routed-view">Final Routed Layout</a></li>
      <li><a href="#day5-routed-zoom">Zoomed-In Routed View</a></li>
      <li><a href="#day5-picorv32-def">picorv32a Final DEF (PNG)</a></li>
      <li><a href="#day5-openroad-start">OpenROAD Flow – Start</a></li>
      <li><a href="#day5-openroad-end">OpenROAD Flow – End</a></li>
    </ul>
  </details>
</details>

---

## 📅 Day 1 – OpenLane & Synthesis Flow

<a id="day1-lab-part1"></a>
### 🔬 Lab Day 1

| Part | Preview |
|--|--|
| Part 1 | ![Lab Day 1 – Part 1](images/day%201%20images/lab%20day%201%20part%201.JPG) |
| Part 2 | ![Lab Day 1 – Part 2](images/day%201%20images/lab%20day%20part%202.JPG) |
| Part 3 | ![Lab Day 1 – Part 3](images/day%201%20images/lab%20day%201%20part%203.JPG) |
| Part 4 | ![Lab Day 1 – Part 4](images/day%201%20images/lab%20day%201%20part%204.JPG) |
| Part 5 | ![Lab Day 1 – Part 5](images/day%201%20images/lab%20day%201%20part%205.JPG) |
| Part 6 | ![Lab Day 1 – Part 6](images/day%201%20images/lab%20day%201%20part%206.JPG) |
| Part 7 | ![Lab Day 1 – Part 7](images/day%201%20images/lab%20day%201%20part%207.JPG) |
| Part 8 | ![Lab Day 1 – Part 8](images/day%201%20images/lab%20day%201%20part%208.JPG) |

---

<a id="day1-openlane-work-dir"></a>
### 🛠️ OpenLane Setup & Execution (Day 1)

- **OpenLane Work Directory**  
  ![OpenLane Work Directory](images/day%201%20images/openlane%20work%20directory%20day%201.JPG)

<a id="day1-openlane-launch"></a>
- **OpenLane Launch**  
  ![OpenLane Open](images/day%201%20images/day%201%20lab%20openlane%20open.JPG)

<a id="day1-config-tcl"></a>
- **`config.tcl` File**  
  ![config.tcl File](images/day%201%20images/day%201%20lab%20config.tcl%20fike.JPG)

<a id="day1-prep-design"></a>
- **Design Preparation – `picorv32a`**  
  ![Prep Design – picorv32a](images/day%201%20images/day%201%20lab%20prep%20-design%20picorv32a.JPG)

<a id="day1-new-runs"></a>
- **New Runs Directory Created**  
  ![New Runs File Created](images/day%201%20images/day%201%20lab,%20new%20runs%20file%20created.JPG)

<a id="day1-results-folder"></a>
- **Results Folder**  
  ![Results Folder](images/day%201%20images/results%20folder%20day%201%20lab.JPG)

<a id="day1-success-synth"></a>
- **✅ Successful Synthesis**  
  ![Successful Synthesis](images/day%201%20images/successful%20synthesis.JPG)

<a id="day1-ff-count"></a>
- **🔢 Flip-Flop Count: 1613**  
  ![Number of Flip-Flops](images/day%201%20images/no%20of%20ff%201613%20day%201.JPG)

<a id="day1-ff-ratio-final"></a>
- **📊 FF Ratio (Final)**  
  ![FF Ratio (Final)](images/day%201%20images/ff%20ratio%20final%20day%201.JPG)

<a id="day1-ff-ratio-pct"></a>
- **📊 FF Ratio (Percentage)**  
  ![FF Ratio (Percentage)](images/day%201%20images/ff%20ratio%20in%20percentage%20day%201.JPG)

<a id="day1-netlist-runs"></a>
- **📄 Synthesized Netlist (Runs Folder)**  
  ![Synthesized Netlist](images/day%201%20images/synthesised%20netlist%20in%20runs%20folder.JPG)

<a id="day1-netlist-gedit"></a>
- **📄 Synthesized Netlist (Gedit View)**  
  ![Netlist in Gedit](images/day%201%20images/synthesised%20netlist%20in%20gedit%20day%201.JPG)

<a id="day1-yosys-stats"></a>
- **📈 Yosys Statistics Report**  
  ![Yosys Stats](images/day%201%20images/yosys%20statistics%20report%20day%201.JPG)

<a id="day1-yosys-stats-gedit"></a>
- **📈 Yosys Stats (Gedit View)**  
  ![Yosys Stats in Gedit](images/day%201%20images/yosys%20stats%20report%20gedit%20day%201.JPG)

<a id="day1-available-reports"></a>
- **📋 Available Reports**  
  ![Available Reports](images/day%201%20images/different%20available%20reports%20day%201.JPG)

<a id="day1-opensta-timing"></a>
- **⏱️ OpenSTA Timing Report**  
  ![OpenSTA Timing](images/day%201%20images/opensta%20timing%20day%201.JPG)

---

## 📅 Day 2 – Floorplanning, Power Planning & Placement

<a id="day2-decap"></a>
### 📖 Theory Concepts

- **Decoupling Capacitors**  
  ![Decoupling Capacitors](images/day%202%20images/theory%20decoupling%20cap.JPG)

<a id="day2-decap-example"></a>
- **Decoupling Capacitor – Example**  
  ![Decap Example](images/day%202%20images/decap%202.JPG)

<a id="day2-ground-bounce"></a>
- **Ground Bounce**  
  ![Ground Bounce](images/day%202%20images/day%202%20ground%20bounce.JPG)

<a id="day2-voltage-droop"></a>
- **Voltage Droop**  
  ![Voltage Droop](images/day%202%20images/voltage%20droop.JPG)

<a id="day2-droop-solution"></a>
- **Solution to Voltage Droop**  
  ![Voltage Droop Solution](images/day%202%20images/solution%20to%20voltage%20droop..JPG)

<a id="day2-multi-supply"></a>
- **Multiple Supplies & Grounds**  
  ![Multi-Supply Solution](images/day%202%20images/solution%20to%20voltage%20droop-%20multiple%20supplies%20and%20grounds.JPG)

<a id="day2-power-plan"></a>
- **Power Planning & Meshes**  
  ![Power Planning](images/day%202%20images/power%20planning%20and%20meshes.JPG)

---

<a id="day2-design-to-place"></a>
### 🧱 Design & Floorplanning

- **Design to be Placed**  
  ![Design](images/day%202%20images/day%202%20design%20to%20be%20placed.JPG)

<a id="day2-port-placement"></a>
- **Port Placement on Die**  
  ![Port Placement](images/day%202%20images/port%20placement%20on%20die.JPG)

<a id="day2-ready-pnr"></a>
- **Ready for PnR**  
  ![Ready for PnR](images/day%202%20images/ready%20for%20pnr.JPG)

<a id="day2-config-readme"></a>
- **Config README**  
  ![Config README](images/day%202%20images/config%20readme.JPG)

<a id="day2-core-util"></a>
- **Floorplanning & Core Utilization**  
  ![Core Utilization](images/day%202%20images/floorplanning%20and%20core%20utilisation%20in%20config%20readme.JPG)

<a id="day2-floorplan-tcl"></a>
- **`floorplan.tcl` Script**  
  ![Floorplan TCL](images/day%202%20images/floorplan%20tcl.JPG)

<a id="day2-design-config"></a>
- **Design Config Files**  
  ![Design Config Files](images/day%202%20images/design%20config%20files.JPG)

<a id="day2-config-in-folder"></a>
- **`config.tcl` in Design Folder**  
  ![Config in Design Folder](images/day%202%20images/config%20tcl%20in%20design%20folder.JPG)

---

<a id="day2-success-floorplan"></a>
### 🏗️ Floorplan Output

- **✅ Successful Floorplan**  
  ![Successful Floorplan](images/day%202%20images/successful%20floorplan.JPG)

<a id="day2-floorplan-def-png"></a>
- **Floorplan DEF (PNG)**  
  ![Floorplan DEF PNG](images/day%202%20images/floorplan%20def%20png.JPG)

<a id="day2-floorplan-def-gedit"></a>
- **Floorplan DEF (Gedit)**  
  ![Floorplan DEF Gedit](images/day%202%20images/flooplan%20def%20gedit.JPG)

<a id="day2-magic-floorplan"></a>
- **Magic Output – Floorplan**  
  ![Magic Floorplan](images/day%202%20images/magic%20output%20of%20floorplan.JPG)

<a id="day2-pin-select"></a>
- **Pin Selection in Magic**  
  ![Pin Selection](images/day%202%20images/pin%20select%20magic.JPG)

<a id="day2-std-cells-pre"></a>
- **Std Cells Visible Pre-Placement**  
  ![Std Cells Before Placement](images/day%202%20images/presence%20of%20std%20cells%20in%20lower%20left%20even%20before%20placement.JPG)

<a id="day2-post-floorplan-magic"></a>
- **Post-Floorplan Magic View**  
  ![Post-Floorplan Magic](images/day%202%20images/post%20floorplan%20magic%20view.JPG)

---

<a id="day2-sta-slide"></a>
### 📍 Placement Phase

- **STA Slide**  
  ![STA Slide](images/day%202%20images/sta%20slide.JPG)

<a id="day2-success-placement"></a>
- **✅ Successful Placement**  
  ![Successful Placement](images/day%202%20images/successful%20placement.JPG)

<a id="day2-placement-output"></a>
- **Placement Run Output Directory**  
  ![Placement Output Dir](images/day%202%20images/placement%20run%20output%20dir.JPG)

<a id="day2-picorv32-placement"></a>
- **`picorv32` Post-Placement View**  
  ![picorv32 Placement](images/day%202%20images/pciorv32%20post%20placement%20png.JPG)

<a id="day2-magic-floorplan-tool"></a>
- **Magic – Floorplan (Tool View)**  
  ![Magic Floorplan Tool](images/day%202%20images/magic%20output%20of%20floorplan%20in%20tool.JPG)

<a id="day2-magic-post-place"></a>
- **Magic – Post Placement**  
  ![Magic Post Placement](images/day%202%20images/magic%20output%20post%20placement.JPG)

---

<a id="day2-cell-flow-lecture"></a>
### ⚙️ Cell Design & Characterization Flow

- **Lecture – Cell Design Flow (Post PnR)**  
  ![Cell Design Flow Lecture](images/day%202%20images/lecture%20cell%20design%20flow%20post%20placement%20and%20routing.JPG)

<a id="day2-cell-flow"></a>
- **Cell Design Flow**  
  ![Cell Design Flow](images/day%202%20images/cell%20design%20flow.JPG)

<a id="day2-complete-flow"></a>
- **Complete Cell Design Flow**  
  ![Complete Flow](images/day%202%20images/complete%20cell%20design%20flow.JPG)

<a id="day2-char-flow"></a>
- **Characterization Flow**  
  ![Characterization Flow](images/day%202%20images/characterisation%20flow.JPG)

<a id="day2-model-file"></a>
- **Model File (`.txt`)**  
  ![Model File](images/day%202%20images/model%20file%20txt].JPG)

## 📅 Day 3 – Standard Cell Design, Layout & Characterization

<a id="day3-magic-inverter"></a>
### 🧪 Custom Inverter Design in Magic

- **Magic Custom Inverter**  
  ![Magic Custom Inverter](images/day%203%20images/magic%20custom%20inverter.JPG)

<a id="day3-inverter-layout"></a>
- **Inverter Layout View**  
  ![Magic Custom Inverter Layout](images/day%203%20images/magic%20custom%20inverter%20layout.JPG)

---

<a id="day3-cmos-fab"></a>
### 🔬 CMOS Fabrication & Transistor Identification

- **CMOS Fabrication Process Overview**  
  ![CMOS Fab Process](images/day%203%20images/cmos%20fab%20process.JPG)

<a id="day3-nmos"></a>
- **NMOS Transistor Identified**  
  ![NMOS Identified](images/day%203%20images/nmos%20indentified.JPG)

<a id="day3-pmos"></a>
- **PMOS Transistor Identified**  
  ![PMOS Identified](images/day%203%20images/pmos%20identifies.JPG)

<a id="day3-output-y"></a>
- **Output `Y` Connected to PMOS & NMOS Drains**  
  ![Output Connection](images/day%203%20images/output%20y%20connected%20to%20pmos%20and%20nmos%20drains.JPG)

<a id="day3-pmos-vdd"></a>
- **PMOS Source → VDD**  
  ![PMOS to VDD](images/day%203%20images/pmos%20source%20to%20vdd.JPG)

<a id="day3-nmos-vss"></a>
- **NMOS Source → VSS**  
  ![NMOS to VSS](images/day%203%20images/nmos%20source%20to%20vss.JPG)

---

<a id="day3-drc-error"></a>
### ⚠️ Layout Editing & DRC Validation

- **Deleting Layout to Trigger DRC Error**  
  ![DRC Error Demo](images/day%203%20images/deleting%20necessary%20layout%20to%20see%20drc%20error.JPG)

<a id="day3-drc-understand"></a>
- **Selecting Random Area to Understand DRC Rules**  
  ![DRC Understanding](images/day%203%20images/select%20random%20area%20and%20drc%20why.JPG)

<a id="day3-via-view"></a>
- **Via View in Magic**  
  ![Via View](images/day%203%20images/via%20view%20in%20magic.JPG)

<a id="day3-load-poly"></a>
- **Load Poly Layer in Magic**  
  ![Load Poly](images/day%203%20images/load%20poly%20mag.JPG)

---

<a id="day3-spice-cmd"></a>
### 🔌 SPICE Extraction & Simulation

- **SPICE Extraction Commands**  
  ![SPICE Extraction](images/day%203%20images/spice%20extraction%20commands.JPG)

<a id="day3-spice-file"></a>
- **Generated SPICE Netlist**  
  ![Created SPICE File](images/day%203%20images/created%20spice%20file.JPG)

<a id="day3-spice-explain"></a>
- **SPICE File Explanation**  
  ![SPICE Explanation](images/day%203%20images/explanantion%20of%20spice%20file.JPG)

<a id="day3-grid-meas"></a>
- **Grid Measurement for Layout Scaling**  
  ![Grid Measurement](images/day%203%20images/grid%20measurement.JPG)

<a id="day3-spice-v1"></a>
- **Updated SPICE File – Version 1**  
  ![SPICE v1](images/day%203%20images/updated%20spice%20file%201.JPG)

<a id="day3-spice-v2"></a>
- **Updated SPICE File – Version 2**  
  ![SPICE v2](images/day%203%20images/updated%20spice%20file%202.JPG)

<a id="day3-ngspice-run"></a>
- **Ngspice Simulation Run**  
  ![Ngspice Run](images/day%203%20images/ngspice%20run.JPG)

<a id="day3-waveform"></a>
- **Ngspice Waveform – Inverter Response**  
  ![Inverter Waveform](images/day%203%20images/ngspice%20waveform%20inverter.JPG)

---

<a id="day3-rise-20"></a>
### ⏱️ Timing Analysis from Simulation

- **Rise Time – 20% Point**  
  ![Rise Time 20%](images/day%203%20images/rise%20time%2020%20percent.JPG)

<a id="day3-x-066y"></a>
- **X Value at 0.66·Y (20% of 3.3V)**  
  ![X at 0.66Y](images/day%203%20images/x%20value%20for%20.66%20y%20value.JPG)

<a id="day3-rise-80"></a>
- **Rise Time – 80% Point**  
  ![Rise Time 80%](images/day%203%20images/rise%20time%2080%20percent.JPG)

<a id="day3-x-264y"></a>
- **X Value at 2.64·Y (80% of 3.3V)**  
  ![X at 2.64Y](images/day%203%20images/x%20value%20for%202.64%20y%20value.JPG)

> 💡 **Note**: Rise time = `t₈₀% – t₂₀%` → used for characterization.

---

<a id="day3-skywater-cmd"></a>
### 🛠️ SkyWater PDK & Magic Tech File Exploration

- **Commands to Download & View Corrupted SkyWater Tech File**  
  ![Corrupted Tech File Commands](images/day%203%20images/commands%20to%20download%20and%20view%20corrupted%20skywater%20process%20magic%20tech%20file.JPG)

<a id="day3-met3-files"></a>
- **Metal 3 (M3) Magic Files**  
  ![M3 Files](images/day%203%20images/met3%20magic%20files.JPG)

<a id="day3-met3-layout"></a>
- **Metal 3 Layout View**  
  ![M3 Layout](images/day%203%20images/met%203%20magic%20layout.JPG)

<a id="day3-tech-v1"></a>
- **Edited Tech File – Version 1**  
  ![Tech File v1](images/day%203%20images/edited%20tech%201.JPG)

<a id="day3-tech-v2"></a>
- **Edited Tech File – Version 2**  
  ![Tech File v2](images/day%203%20images/edited%20tech%202.JPG)

<a id="day3-updated-drc"></a>
- **Updated DRC After Tech File Fix**  
  ![Updated DRC](images/day%203%20images/updated%20drc.JPG)

## 📅 Day 4 – Timing Analysis & Clock Tree Synthesis

<a id="day4-tracks"></a>
### 🧩 Setup & Technology Files

- **Tracks Info File**  
  ![Tracks Info File](images/day%204%20images/tracks%20info%20file.JPG)

<a id="day4-lef-ss"></a>
- **LEF File (Slow-Slow Corner – SS)**  
  ![LEF File SS](images/day%204%20images/lef%20file%20ss.JPG)

<a id="day4-copy-lef"></a>
- **Commands to Copy LEF File**  
  ![Copy LEF Commands](images/day%204%20images/copy%20lef%20file%20commands%20run.JPG)

<a id="day4-include-lef"></a>
- **Commands to Include New LEF in Flow**  
  ![Include New LEF](images/day%204%20images/commands%20to%20include%20new%20lef.JPG)

---

<a id="day4-mod-config"></a>
### ⚙️ Design Configuration & Synthesis

- **Modified `config.tcl`**  
  ![Modified Config TCL](images/day%204%20images/modified%20config%20tcl.JPG)

<a id="day4-prep-final"></a>
- **Prep Final Design**  
  ![Prep Final Design](images/day%204%20images/prep%20final%20design.JPG)

<a id="day4-synth1"></a>
- **✅ Successful Synthesis (Initial)**  
  ![Successful Synthesis](images/day%204%20images/successful%20synthesis.JPG)

<a id="day4-synth2"></a>
- **✅ Successful Synthesis – Second Run**  
  ![Successful Synthesis 2](images/day%204%20images/successful%20synthesis2.JPG)

<a id="day4-optimized-synth"></a>
- **✅ Optimized Synthesis Completed**  
  ![Optimized Synthesis](images/day%204%20images/optimised%20synthesis%20successfull.JPG)

<a id="day4-save1"></a>
- **💾 Save Checkpoint #1**  
  ![Save Number 1](images/day%204%20images/save%20number%201.JPG)

---

<a id="day4-fail-floorplan"></a>
### 🏗️ Floorplanning & Placement

- **❌ Failed Initial Floorplan**  
  ![Failed Floorplan](images/day%204%20images/failed%20initial%20floorplan.JPG)

<a id="day4-manual-floorplan"></a>
- **✅ Manual Multi-Step Floorplan Success**  
  ![Manual Floorplan](images/day%204%20images/manual%20multi%20step%20floorplan.JPG)

<a id="day4-placement-done"></a>
- **✅ Placement Completed**  
  ![Placement Done](images/day%204%20images/placement%20done.JPG)

<a id="day4-placement-def"></a>
- **Placement DEF File**  
  ![Placement DEF](images/day%204%20images/placement%20def%20file.JPG)

<a id="day4-custom-cell"></a>
- **Instance of Our Custom Cell in Layout**  
  ![Custom Cell Instance](images/day%204%20images/instance%20of%20our%20custom%20cell.JPG)

<a id="day4-expanded-view"></a>
- **Expanded View of Custom Cell**  
  ![Expanded View](images/day%204%20images/expanded%20view.JPG)

---

<a id="day4-base-sdc"></a>
### ⏱️ Static Timing Analysis (STA)

- **Base SDC Constraints File**  
  ![Base SDC](images/day%204%20images/base%20sdc.JPG)

<a id="day4-pre-sta"></a>
- **Pre-STA Configuration**  
  ![Pre STA Conf](images/day%204%20images/pre%20sta%20conf.JPG)

<a id="day4-sta1"></a>
- **STA Run – Initial**  
  ![STA Run](images/day%204%20images/sta%20run.JPG)

<a id="day4-sta2"></a>
- **STA Run – Second Pass**  
  ![STA Run 2](images/day%204%20images/sta%20run%202.JPG)

<a id="day4-sta-final"></a>
- **STA – Final Verification**  
  ![STA Once More](images/day%204%20images/sta%20once%20more.JPG)

---

<a id="day4-cond1"></a>
### 🔍 Timing Conditions & Optimization

- **✅ Condition 1 Verified**  
  ![Condition 1](images/day%204%20images/condition%201%20verified.JPG)

<a id="day4-cond2"></a>
- **✅ Condition 2 Verified**  
  ![Condition 2](images/day%204%20images/condition%202%20verified.JPG)

<a id="day4-cond3"></a>
- **Condition 3 (Under Evaluation)**  
  ![Condition 3](images/day%204%20images/condition%203.JPG)

<a id="day4-or-fanout"></a>
- **OR Gate with Multiple Fanouts**  
  ![OR Gate Fanout](images/day%204%20images/or%20gate%20multiple%20fanout.JPG)

<a id="day4-cell-opt"></a>
- **Cell Optimization Applied**  
  ![Cell Optimisation](images/day%204%20images/cell%20optimisation.JPG)

<a id="day4-eco"></a>
- **✅ Basic ECO (Engineering Change Order) Complete**  
  ![Basic ECO Complete](images/day%204%20images/basic%20eco%20complete.JPG)

## 📅 Day 5 – Final Steps: CTS, PDN & Routing

<a id="day5-final-place"></a>
### 🧱 Final Placement & Optimization

- **Final Placement View**  
  ![Final Placement](images/day%205%20images/final%20placement.JPG)

<a id="day5-final-opt"></a>
- **Final Optimizations Applied**  
  ![Final Optimisations](images/day%205%20images/final%20optimisations.JPG)

---

<a id="day5-cts"></a>
### ⏱️ Clock Tree Synthesis (CTS)

- **✅ Final Successful CTS**  
  ![Successful CTS](images/day%205%20images/final%20successful%20cts.JPG)

---

<a id="day5-pdn"></a>
### 🔌 Power Delivery Network (PDN)

- **Final PDN Implementation**  
  ![Final PDN](images/day%205%20images/final%20pdn.JPG)

<a id="day5-pdn-def"></a>
- **PDN in DEF Format**  
  ![PDN DEF](images/day%205%20images/pdn%20def.JPG)

<a id="day5-pdn-lines1"></a>
- **PDN Power Lines – View 1**  
  ![PDN Lines](images/day%205%20images/pdn%20lines.JPG)

<a id="day5-pdn-lines2"></a>
- **PDN Power Lines – View 2**  
  ![PDN Lines 2](images/day%205%20images/pdn%20lines%202.JPG)

---

<a id="day5-routing-ongoing"></a>
### 🧭 Global & Detailed Routing

- **Routing in Progress**  
  ![Ongoing Routing](images/day%205%20images/ongoing%20routing.JPG)

<a id="day5-routing-done"></a>
- **✅ Routing Completed**  
  ![Routing Completed](images/day%205%20images/routing%20completed.JPG)

<a id="day5-routed-view"></a>
- **Final Routed Layout**  
  ![Final Routed View](images/day%205%20images/final%20routed%20view.JPG)

<a id="day5-routed-zoom"></a>
- **Zoomed-In Routed View**  
  ![Final Routed Zoomed](images/day%205%20images/final%20routed%20zoomed%20view.JPG)

<a id="day5-picorv32-def"></a>
- **`picorv32a` Final DEF (PNG Export)**  
  ![picorv32a DEF PNG](images/day%205%20images/picorv32a%20def%20png.JPG)

---

<a id="day5-openroad-start"></a>
### 🚀 OpenROAD Flow Execution

- **OpenROAD Flow – Start**  
  ![OpenROAD Start](images/day%205%20images/openroad%20start.JPG)

<a id="day5-openroad-end"></a>
- **OpenROAD Flow – End (RTL-to-GDS Complete!)**  
  ![OpenROAD End](images/day%205%20images/openroad%20end.JPG)
