# CFD Viewer — Interactive 1D/2D Visualization Tool  

**CFD Viewer** is a lightweight, browser-based application for visualizing **Computational Fluid Dynamics (CFD)** datasets.  
It supports both **nozzle/axial flow data** (`X/D`, pressure, Mach number) and **2D field data** (`x, y, u, v`), enabling fast, interactive exploration without the need for heavy post-processing software.  

---

## Key Features
- CSV input support — compatible with exported CFD or experimental data.  
- 1D visualization — plot Mach number, absolute pressure, and total pressure versus `X/D`.  
- 2D visualization — generate contour maps of velocity magnitude, pressure, or scalar fields.  
- Vector plots — display velocity fields with adjustable arrow downsampling.  
- Export options — save plots as high-resolution PNGs for reports and presentations.  
- Demo dataset — test the viewer instantly without uploading any files.  

---

## Getting Started

1. Clone or download this repository:  
   ```bash
   git clone https://github.com/NeethuVelangi/cfd-viewer.git
   ```
2. Open `cfd_viewer.html` (for 2D datasets) or `cfd_viewer_axial.html` (for nozzle/axial flow datasets) in your browser.  
3. Upload your CSV file containing the required headers:  

   - **Nozzle/Axial flow data**: `X/D, AP, TP(PASCAL), MN`  
   - **2D field data**: `x, y, u, v` (+ optional `phi`)  

---

## Example CSV Formats

### Nozzle Flow Data
```csv
X, X/D, AP, TP, TP(PASCAL), MN
0.0,0.0,101325,101325,101325,0.0
0.1,0.1,100000,101300,101300,0.1
0.2,0.2,95000,101200,101200,0.2
```

### 2D Field Data
```csv
x,y,u,v,phi
0.0,0.0,0.0,0.0,0.1
0.1,0.0,0.2,0.05,0.12
```

---

## Applications
- Rapid CFD project visualization  
- Nozzle flow analysis (Mach/pressure distributions)  
- Educational demonstrations and research presentations  
- Quick validation of CFD solver outputs  

---

## Roadmap
Planned improvements include:  
- Support for multiple variable overlays  
- Handling of time-dependent datasets  
- Customizable colormaps  
- Advanced interpolation for irregular grids  

---

## Author
**[Neethusri Velangi](https://github.com/NeethuVelangi)**  
Aeronautical Engineering student with interests in CFD, propulsion, and aerospace systems.  

---

## License
This project is shared for educational and research purposes.  
Feel free to use, modify, and adapt it to your needs.  

