---
{"dg-publish":true,"permalink":"/py-mol/6-scripting/","title":"Exercise 6: PyMOL Scripting and Automation"}
---

# PyMOL Exercise 5: PyMOL Scripting and Automation

This exercise teaches you how to move from the GUI to reproducible **.pml scripts**. Scripting allows you to automate repetitive tasks and ensure your visualizations can be recreated exactly.

---

## **Step 1: Create a basic .pml script**

A PyMOL script is just a list of commands saved in a text file with the `.pml` extension.

1. Open a text editor (VS Code, Textadept).
2. Create a new file named `mcherry_style.pml`.
3. Add the following commands and expand:

```pymol
# mcherry_style.pml

# 1. Fetch the structure
fetch 2H5Q
hide everything
...
```

4. Save and include a view.
---

## **Step 4: Challenge - The "Figure Generator" Script**

Create a script that performs the following:
1. Downloads a structure of your choice.
2. Colors it according to **B-factor** (experimental flexibility).
3. Adds a surface with 70% transparency.
4. Ray traces the image and saves it automatically.

```pymol
# Example for Step 4
spectrum b, blue_white_red
ray 1600, 1200
png my_publication_figure.png
```

Alternatively, be creative and write your own script.
### Summary

1. Write and execute **.pml scripts** for reproducibility.
2. Automate **loading, representing, and coloring** of proteins.
3. Understand how to mix **PyMOL commands and Python code**.
4. Generate **standardized output (PNGs)** via scripts.

---

[[PyMOL/5_mcherry_intein\|← Previous]] | [[PyMOL/7_animations_movies\|Next →]]
