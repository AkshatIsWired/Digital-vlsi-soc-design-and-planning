# 🧠 Digital VLSI SoC Design and Planning

> 📚 Documentation of my learning journey through this course on **Digital VLSI System-on-Chip (SoC) Design and Planning**.

---

<details>
  <summary><strong>📘 Day-wise Digital VLSI SoC Design Journey (Click to Expand)</strong></summary>

  <ul>
    <li>
      <a href="images/day%201%20images">
        📅 Day 1 – Open-source EDA, OpenLANE & RTL-to-GDS Overview
      </a>
    </li>
    <li>
      <a href="images/day%202%20images">
        📅 Day 2 – Floorplanning, Placement & Library Characterization
      </a>
    </li>
    <li>
      <a href="images/day%203%20images">
        📅 Day 3 – Standard Cell Design & SPICE Characterization
      </a>
    </li>
    <li>
      <a href="images/day%204%20images">
        📅 Day 4 – Timing Analysis & Clock Tree Synthesis
      </a>
    </li>
    <li>
      <a href="images/day%205%20images">
        📅 Day 5 – Routing, DRC & Final RTL-to-GDS Closure
      </a>
    </li>
  </ul>

</details>

---

## 📅 Day 1 – OpenLane & Synthesis Flow

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

### 🛠️ OpenLane Setup & Execution (Day 1)

- **OpenLane Work Directory**  
  ![OpenLane Work Directory](images/day%201%20images/openlane%20work%20directory%20day%201.JPG)

- **OpenLane Launch**  
  ![OpenLane Open](images/day%201%20images/day%201%20lab%20openlane%20open.JPG)

- **`config.tcl` File**  
  ![config.tcl File](images/day%201%20images/day%201%20lab%20config.tcl%20fike.JPG)

- **Design Preparation – `picorv32a`**  
  ![Prep Design – picorv32a](images/day%201%20images/day%201%20lab%20prep%20-design%20picorv32a.JPG)

- **New Runs Directory Created**  
  ![New Runs File Created](images/day%201%20images/day%201%20lab,%20new%20runs%20file%20created.JPG)

- **Results Folder**  
  ![Results Folder](images/day%201%20images/results%20folder%20day%201%20lab.JPG)

- **✅ Successful Synthesis**  
  ![Successful Synthesis](images/day%201%20images/successful%20synthesis.JPG)

- **🔢 Flip-Flop Count: 1613**  
  ![Number of Flip-Flops](images/day%201%20images/no%20of%20ff%201613%20day%201.JPG)

- **📊 FF Ratio (Final)**  
  ![FF Ratio (Final)](images/day%201%20images/ff%20ratio%20final%20day%201.JPG)

- **📊 FF Ratio (Percentage)**  
  ![FF Ratio (Percentage)](images/day%201%20images/ff%20ratio%20in%20percentage%20day%201.JPG)

- **📄 Synthesized Netlist (Runs Folder)**  
  ![Synthesized Netlist](images/day%201%20images/synthesised%20netlist%20in%20runs%20folder.JPG)

- **📄 Synthesized Netlist (Gedit View)**  
  ![Netlist in Gedit](images/day%201%20images/synthesised%20netlist%20in%20gedit%20day%201.JPG)

- **📈 Yosys Statistics Report**  
  ![Yosys Stats](images/day%201%20images/yosys%20statistics%20report%20day%201.JPG)

- **📈 Yosys Stats (Gedit View)**  
  ![Yosys Stats in Gedit](images/day%201%20images/yosys%20stats%20report%20gedit%20day%201.JPG)

- **📋 Available Reports**  
  ![Available Reports](images/day%201%20images/different%20available%20reports%20day%201.JPG)

- **⏱️ OpenSTA Timing Report**  
  ![OpenSTA Timing](images/day%201%20images/opensta%20timing%20day%201.JPG)

---

## 📅 Day 2 – Floorplanning, Power Planning & Placement

### 📖 Theory Concepts

- **Decoupling Capacitors**  
  ![Decoupling Capacitors](images/day%202%20images/theory%20decoupling%20cap.JPG)

- **Decoupling Capacitor – Example**  
  ![Decap Example](images/day%202%20images/decap%202.JPG)

- **Ground Bounce**  
  ![Ground Bounce](images/day%202%20images/day%202%20ground%20bounce.JPG)

- **Voltage Droop**  
  ![Voltage Droop](images/day%202%20images/voltage%20droop.JPG)

- **Solution to Voltage Droop**  
  ![Voltage Droop Solution](images/day%202%20images/solution%20to%20voltage%20droop..JPG)

- **Multiple Supplies & Grounds**  
  ![Multi-Supply Solution](images/day%202%20images/solution%20to%20voltage%20droop-%20multiple%20supplies%20and%20grounds.JPG)

- **Power Planning & Meshes**  
  ![Power Planning](images/day%202%20images/power%20planning%20and%20meshes.JPG)

---

### 🧱 Design & Floorplanning

- **Design to be Placed**  
  ![Design](images/day%202%20images/day%202%20design%20to%20be%20placed.JPG)

- **Port Placement on Die**  
  ![Port Placement](images/day%202%20images/port%20placement%20on%20die.JPG)

- **Ready for PnR**  
  ![Ready for PnR](images/day%202%20images/ready%20for%20pnr.JPG)

- **Config README**  
  ![Config README](images/day%202%20images/config%20readme.JPG)

- **Floorplanning & Core Utilization**  
  ![Core Utilization](images/day%202%20images/floorplanning%20and%20core%20utilisation%20in%20config%20readme.JPG)

- **`floorplan.tcl` Script**  
  ![Floorplan TCL](images/day%202%20images/floorplan%20tcl.JPG)

- **Design Config Files**  
  ![Design Config Files](images/day%202%20images/design%20config%20files.JPG)

- **`config.tcl` in Design Folder**  
  ![Config in Design Folder](images/day%202%20images/config%20tcl%20in%20design%20folder.JPG)

---

### 🏗️ Floorplan Output

- **✅ Successful Floorplan**  
  ![Successful Floorplan](images/day%202%20images/successful%20floorplan.JPG)

- **Floorplan DEF (PNG)**  
  ![Floorplan DEF PNG](images/day%202%20images/floorplan%20def%20png.JPG)

- **Floorplan DEF (Gedit)**  
  ![Floorplan DEF Gedit](images/day%202%20images/flooplan%20def%20gedit.JPG)

- **Magic Output – Floorplan**  
  ![Magic Floorplan](images/day%202%20images/magic%20output%20of%20floorplan.JPG)

- **Pin Selection in Magic**  
  ![Pin Selection](images/day%202%20images/pin%20select%20magic.JPG)

- **Std Cells Visible Pre-Placement**  
  ![Std Cells Before Placement](images/day%202%20images/presence%20of%20std%20cells%20in%20lower%20left%20even%20before%20placement.JPG)

- **Post-Floorplan Magic View**  
  ![Post-Floorplan Magic](images/day%202%20images/post%20floorplan%20magic%20view.JPG)

---

### 📍 Placement Phase

- **STA Slide**  
  ![STA Slide](images/day%202%20images/sta%20slide.JPG)

- **✅ Successful Placement**  
  ![Successful Placement](images/day%202%20images/successful%20placement.JPG)

- **Placement Run Output Directory**  
  ![Placement Output Dir](images/day%202%20images/placement%20run%20output%20dir.JPG)

- **`picorv32` Post-Placement View**  
  ![picorv32 Placement](images/day%202%20images/pciorv32%20post%20placement%20png.JPG)

- **Magic – Floorplan (Tool View)**  
  ![Magic Floorplan Tool](images/day%202%20images/magic%20output%20of%20floorplan%20in%20tool.JPG)

- **Magic – Post Placement**  
  ![Magic Post Placement](images/day%202%20images/magic%20output%20post%20placement.JPG)

---

### ⚙️ Cell Design & Characterization Flow

- **Lecture – Cell Design Flow (Post PnR)**  
  ![Cell Design Flow Lecture](images/day%202%20images/lecture%20cell%20design%20flow%20post%20placement%20and%20routing.JPG)

- **Cell Design Flow**  
  ![Cell Design Flow](images/day%202%20images/cell%20design%20flow.JPG)

- **Complete Cell Design Flow**  
  ![Complete Flow](images/day%202%20images/complete%20cell%20design%20flow.JPG)

- **Characterization Flow**  
  ![Characterization Flow](images/day%202%20images/characterisation%20flow.JPG)

- **Model File (`.txt`)**  
  ![Model File](images/day%202%20images/model%20file%20txt].JPG)
