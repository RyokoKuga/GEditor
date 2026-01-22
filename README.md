# 🧪 GfEditer - Dual Mode Molecular Editer

README in [Japanese](https://github.com/RyokoKuga/GfEditor/blob/main/README-ja.md)

**GfEditer** is a high-performance web-based tool designed to bridge the gap between **molecular structural modeling** and **GAMESS** input file (`.inp`) generation.

---

## 🌟 Key Features

| Feature | Details |
| :--- | :--- |
| 🔄 **Dual Mode** | Instantly switch between **Modeling** (design) and **Editor** (configuration) modes. |
| ⚡ **Real-time Sync** | Automatically updates XYZ coordinates as you modify the structure, eliminating input errors. |
| ⚛️ **3D Optimizer** | Generates high-precision initial 3D structures from 2D sketches using MMFF94 force field. |
| 📑 **Smart Formatting** | Outputs coordinates with precise column alignment based on GAMESS standards. |

---

## 🛠 Functionalities

### 🎨 Modeling Mode (Molecular Design)
*   **2D Composer**: Build molecules using an intuitive sketching interface.
*   **3D View & Gen**: Click `Generate 3D` to create optimized spatial structures with full 360° rotation.
*   **OpenBabel Integration**: Supports advanced structural conversions and various file formats.

### ⚙️ Editor Mode (Calculation Setup)
*   **Config Panel**: Automatically generates keywords by selecting parameters from dropdown menus.
    *   **Run Type**: `OPTIMIZE`, `ENERGY`, `HESSIAN`, `SADPOINT`, `IRC`.
    *   **Theory**: `RHF`, `UHF`, `B3LYP (DFT)`, `MP2`.
    *   **Basis Sets**: Options ranging from `STO-3G` to `6-31+G(d,p)`.
*   **Dynamic Logic**: Automatically inserts specific control blocks such as `$FORCE`, `$STATPT`, and `$IRC` based on the selected Run Type.
*   **Editable Text**: The generated script is fully editable, allowing for manual refinements or deletions.

---

## 🚀 Workflow

1.  **Draft**: Sketch your molecule in `Modeling Mode` and click `Generate 3D` to obtain coordinates.
2.  **Configure**: Switch to `Editor Mode` and select your computational theory and basis set.
3.  **Download**: Review the generated content and click `Download .inp File` to save your configuration.

---

## 📦 Libraries Used

This project is powered by the following open-source libraries:
*   [Kekule.js](https://github.com/partridgejiang/Kekule.js) - Molecular manipulation engine
*   [Three.js](https://threejs.org) - 3D rendering
*   [Raphael.js](https://github.com/DmitryBaranovskiy/raphael) - 2D graphics support

---

## 📄 License

Copyright © 2026 GfEditer Project.
Licensed under the [MIT License](LICENSE).

---
*Developed for the Computational Chemistry Community.*
