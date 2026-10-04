# Physics-2-group-AI-simulation-Lab
# ⚡ Interactive 2D Electric Field & Potential Simulator

An interactive web-based physics simulation that visualizes electric field vectors, equipotential voltage heatmaps, and test charge forces in real time using Coulomb's Law and Superposition.

🚀 **[Click Here to Open the Live Simulation](https://<YOUR-GITHUB-USERNAME>.github.io/<YOUR-REPO-NAME>/)**

---

## ✨ Features
- **Dynamic Charge Placement**: Add custom protons ($+1e$) and electrons ($-1e$) across a 2D canvas.
- **Electric Field Vectors**: Computes total field magnitude $E$ and components $E_x, E_y$ at any spatial point.
- **Electric Potential (Voltage)**: Renders a dynamic background heatmap representing scalar potential $V$.
- **Test Charge Probe**: Measure electrostatic force $\vec{F} = q_{test}\vec{E}$, angle $\theta$, and individual field values.
- **Presets**: Built-in configurations for Dipole, Quadrupole, Parallel Plate Capacitor, and Point Charges.
- **Database Persistence**: Save charge configurations online using Supabase (or fallback to browser local storage).

---

## 🧮 Physics Principles & Equations

### 1. Electric Field (Coulomb's Law)
For $N$ point charges, the total electric field vector at position $\vec{r}$ is calculated using vector superposition:
$$\vec{E}(\vec{r}) = \sum_{i=1}^{N} k \frac{q_i}{|\vec{r} - \vec{r}_i|^2} \hat{u}_i$$

### 2. Electrostatic Force
The force exerted on a test charge $q_{test}$ placed inside the field:
$$\vec{F} = q_{test} \cdot \vec{E}$$

### 3. Electric Potential (Voltage)
The electric potential $V$ at any coordinate is the scalar sum of contributions:
$$V(\vec{r}) = \sum_{i=1}^{N} k \frac{q_i}{|\vec{r} - \vec{r}_i|}$$

---

## 🛠️ Built With
- **HTML5 Canvas & JavaScript (ES6)**
- **TailwindCSS** for UI layout
- **Supabase JS Client** for cloud database storage
- **GitHub Pages** for free public hosting
