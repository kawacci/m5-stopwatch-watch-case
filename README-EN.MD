# M5Stopwatch Watch Case

**English** | [日本語](./README.MD)

Custom 3D model data for mounting the M5Stack official stopwatch (M5Stopwatch) as a wristwatch.

---

## 📌 Overview

This design securely and smartly mounts the M5Stopwatch using its built-in **magnets** and **strap holder holes**.
The base model was reverse-engineered based on the STL data provided in M5Stack's official hardware repository ([M5Stack/M5_Hardware](https://github.com/m5stack/M5_Hardware)).

* **Band Width Variations**: 20mm / 22mm / 24mm
* **Recommended Printing Method**: Designed primarily for SLA (Stereolithography). FDM (Fused Deposition Modeling) is also possible; please modify the `STEP` data as needed if printing with FDM.

---

## 🧲 Mounting & Parts

* **Magnet**: Daiso "Super Strong Magnet Mini (No.371) 6mm dia. x 3mm thickness" [product link](https://jp.daisonet.com/products/4549131156621)
* Utilizes the magnets and strap holder fixing holes on the back of the device.

---

## 📂 Data Structure & Variations

Both `STL` and `STEP` formats are provided to suit your needs.

### 1. Tough Gear Style Protector Model (G Series)

A snap-fit protector model featuring a rugged design.

#### 🔹 Asymmetric (Offset) Model ★NEW
An offset lug design that prevents the case from digging into the back of your hand when bending your wrist with the larger protector. Choose `L` (Left Offset) or `R` (Right Offset) depending on which wrist you wear it on and your preference.

| Model Name | Description | Preview |
| :--- | :--- | :--- |
| **BANDBASE-G-Offset**<br>`BANDBASE-SIDE[20/22/24]_[L/R].stl` | Asymmetric base designed to avoid hand interference<br>(Band width: 20/22/24mm × L/R, 6 models in total) | ![BANDBASE-G-24mm_L](img/BANDBASE-G-24mm_L.png) |

---

#### 🔹 Standard Center Model
| Model Name | Description | Preview |
| :--- | :--- | :--- |
| **BANDBASE-G**<br>`BANDBASE-G-[20/22/24]mm.stl` | Protector-compatible standard watch base (20/22/24mm) | ![BANDBASE-G](img/BANDBASE-G-24mm.png) |
| **COVER-G** | Protector cover with M5 logo | ![COVER-G](img/COVER-G.png) |
| **COVER-G-none** | Protector cover without logo | ![COVER-G-none](img/COVER-G-none.png) |
| **StopWatch-G (ASSY)** | Overall assembly view with protector attached | ![StopWatch-G](img/StopWatch-G.png) |

---

### 2. Standard & Legacy Models (Original)

| Model Name | Description | Preview (Single / ASSY) |
| :--- | :--- | :--- |
| **BANDBASE1** | Initial model watch base | ![BANDBASE1](img/BANDBASE1.png) ![BANDBASE1_ASSY](img/BANDBASE1_ASSY.png) |
| **BANDBASE2 / 2A** | Improved model for better arm fit (2A includes air vent holes) | ![BANDBASE2](img/BANDBASE2.png) ![BANDBASE2_ASSY](img/BANDBASE2_ASSY.png) |
| **BASE** | Base model without band attachment points | ![BASE](img/BASE.png) ![BASE_ASSY](img/BASE_ASSY.png) |

---

## 🖨️ FDM Printing Reference
Example slice layout when printing with FDM (Fused Deposition Modeling). Adjust supports and orientation as needed.

![FDM Slice Example](img/FDM.png)

---

## 🎬 3D View & Preview Videos
* [BANDBASE1 Video](MOV/BANDBASE1.mov)
* [BANDBASE2 Video](MOV/BANDBASE2.mov)

---

## 📁 Directory Structure

```text
m5-stopwatch-watch-case/
├── img/                  # Preview images
├── LICENSE/              # License files
│   └── LICENSE.txt
├── MOV/                  # 3D model videos
├── STEP/                 # STEP data (for CAD editing)
│   ├── BANDBASE1.step
│   ├── BANDBASE2.step
│   ├── BANDBASE2A.step
│   ├── BASE.step
│   ├── StopWatch.step
│   └── StopWatch_RealReverse.STEP
└── STL/                  # STL data for 3D printing
    ├── BANDBASE-G/        # Protector-compatible standard bases (20/22/24mm)
    ├── BANDBASE-G-Offset/ # Offset bases to avoid hand interference (20/22/24mm × L/R)
    ├── COVER-G/          # Protector covers (with/without logo)
    └── Original/         # Legacy & standard base models

```

## 👤 Author
- Kawacci


## 📄 License
- This repository is published under the [MIT License](/LICENSE/LICENSE.txt) .