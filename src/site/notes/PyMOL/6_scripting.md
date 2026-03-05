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
3. Add the following commands:

```pymol
# mcherry_style.pml

# 1. Fetch the structure
fetch 2H5Q
hide everything

# 2. Set up representations
show cartoon, 2H5Q
show surface, 2H5Q
set transparency, 0.5

# 3. Coloring
color white, 2H5Q
select chromophore, resn CH6
show sticks, chromophore
color magenta, chromophore

# 4. Rendering settings
bg_color white
set antialias, 2
set ray_trace_mode, 1

# 5. Final view
orient
```

---

## **Step 2: Run the script in PyMOL**

There are two ways to execute your script:

Go to `File > Run Script...` and select `mcherry_style.pml`.


---

## **Step 3: Advanced Automation**

You can also use **Python** directly within your scripts for more complex logic.

```python
python
from pymol import cmd

# Count the number of Alpha Carbons
count = cmd.count_atoms("name CA")
print(f"Structure 2H5Q has {count} residues.")

python end
```

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

Alternatively, be creative and come up with your own script.
### Summary

1. Write and execute **.pml scripts** for reproducibility.
2. Automate **loading, representing, and coloring** of proteins.
3. Understand how to mix **PyMOL commands and Python code**.
4. Generate **standardized output (PNGs)** via scripts.

---

[[PyMOL/5_mcherry_intein\|← Previous]]
