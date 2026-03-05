---
{"dg-publish":true,"permalink":"/py-mol/1-pdb-intro/","title":"Exercise 1: PyMOL Introduction"}
---

# PyMOL Exercise 1: Introduction and PDB Exploration

## **What is PyMOL?**

**PyMOL** is a powerful, user-sponsored molecular visualization system used for viewing, rendering, and analyzing 3D structures of biological macromolecules such as proteins, DNA, RNA, and small molecules. It is built on an open-source foundation (Python) and is the gold standard for creating publication-quality images and animations in structural biology.

### **What is PyMOL used for?**
- **Visualization:** Interactively rotate, zoom, and inspect molecular details.
- **Analysis:** Measure distances, identify hydrogen bonds, and analyze surface properties.
- **Rendering:** Generate high-resolution, ray-traced images for journals and presentations.
- **Scripting:** Automate complex tasks using Python or PyMOL's command language (.pml scripts).

---
## **Installation Guide: Open-Source PyMOL (via Miniconda)**

Follow these instructions to install the open-source version of PyMOL using the **Miniconda** package manager. This method is the most reliable way to manage dependencies across different operating systems.

If you do not want to install PyMOL with the Miniconda environment, try the portable versions available on the [Shared Sciebo folder](https://uni-duesseldorf.sciebo.de/s/AQNWFnw45HqJKQe).

### **Step 1: Install Miniconda**

1. **Download:** Visit the [Miniconda Download Page](https://docs.anaconda.com/miniconda/miniconda-other-installer-links/) and download the installer for your operating system:
   - **macOS:** Choose the `pkg` or `sh` installer (select `Apple M1/M2/M3` for modern Macs or `Intel` for older ones).
   - **Windows:** Choose the `Windows 64-bit` installer.
1. **Install:** Run the installer and follow the prompts. Do not add Miniconda to your PATH if prompted; you can simply use the "Anaconda Prompt" created after installation.

### **Step 2: Install PyMOL**

Open your terminal (macOS) or **Anaconda Prompt** (Windows) and run the following commands:

```bash
# 1. Create a new environment named 'pymol' and install the program
conda create -n pymol -c conda-forge pymol -y

# 2. Activate the environment
conda activate pymol

# 3. Launch PyMOL
pymol
```

### **Step 3: Launching PyMOL in the future**

Whenever you want to use PyMOL again, simply open your terminal/prompt and type:
```bash
conda activate pymol
pymol
```

*Note: Please bring a computer mouse to the course for efficient navigation!*

---

## **Step 1: Visit the RCSB PDB**

1. Go to [https://www.rcsb.org/](https://www.rcsb.org/).
2. Identify one of the **"Molecules of the Month"** on the homepage.
3. Note down its **4-digit PDB code** (e.g., `1MBO`, `4HHB`).

---

## **Step 2: Inspect the PDB Header**

Before looking at the 3D model, it is crucial to understand the experimental data.

1. Download the structure coordinate file in **PDB format**.
2. Open the file using a **text editor** (e.g., Textadept, Zed).
3. Look for the following information in the header:
    - **Experimental Method:** Was it solved using `X-RAY DIFFRACTION` or `CRYO-ELECTRON MICROSCOPY`?
    - **Resolution:** Identify the high-resolution cutoff (look for `RESOLUTION RANGE HIGH` or `EFFECTIVE RESOLUTION` in Ångströms).
    - **Quality Metrics:** Identify the `R` and `FREE R` values (for X-ray) or the `NUMBER OF PARTICLES` (for Cryo-EM).
    - **Chains:** How many molecules/chains does the structure coordinate file contain?

> [!figure] #fig:yourfigurelabel width=100% align=center pos=!ht
> ![](/img/user/figures/pdb.png)
>
> PDB file data columns.

---

## **Step 3: Load into PyMOL**

Now, visualize the structure you just inspected.

```pymol
# Option 1: Load the file you downloaded (or drag & drop)
load path/to/your/file.pdb

# Option 2: Fetch directly from the PDB (replace xxxx with your code)
fetch xxxx

# Color by chain to see the individual molecules
color bychain
```

- If you need to start over:
```pymol
# Delete the current object
delete xxxx

# Alternatively, reset PyMOL entirely 
reinitialize

# Reload
fetch xxxx
```

In the command line, use the keyboard arrow buttons ↑ and ↓. What happens?

---
### Summary

1. Navigate the **RCSB PDB** interface.
2. Understand the **metadata** contained in a PDB header (Resolution, R-factors).
3. Differentiate between **X-ray** and **Cryo-EM** structural data.
4. Perform basic **loading and coloring** in PyMOL.

---

[[PyMOL/2_pymol_basics\|Next →]]
