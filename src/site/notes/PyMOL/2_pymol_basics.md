---
{"dg-publish":true,"permalink":"/py-mol/2-pymol-basics/","title":"Exercise 2: PyMOL Basic Navigation"}
---

# PyMOL Exercise 2: Navigation, Selections, and Surfaces

This exercise covers the core mechanics of PyMOL: how to move around, how to select specific parts of a protein using logic, and how to visualize molecular surfaces.

---

## **Step 1: Fetch and Navigate**

```pymol
# Fetch Myoglobin
fetch 1mbo

# Enable the sequence view
set seq_view, 1
```

Alternatively, Display → Show Sequence or the `S` button in the lower right corner.

Click on individual residues in the sequence view. They will be selected in the structure view.
### **Navigation Controls:**
- **Rotate:** Left-click and drag.
- **Zoom:** Right-click and drag.
- **Pan (Move):** Middle-click (scroll wheel) and drag.

---

## **Step 2: Basic Representations**

Experiment with different ways to show the protein chain:

Use the **(H)ide** and **(S)how** buttons of the loaded structure.

Alternatively:
```pymol
# Hide everything first
hide everything, all

# Show as sticks
show sticks, all

# Show as ribbon
show ribbon, all

# Show as cartoon (Standard for proteins)
show cartoon, all
```

Experiment with different ways to show the protein chain using the **(S)how** and **(H)ide** buttons. Experiment with the **(C)olor** button.

---

## **Step 3: Advanced Selection Logic**

PyMOL uses a powerful selection language. We will isolate the **Heme** group and its environment.

```pymol
# set a white background
bg_color white

# Select the Heme ligand
select ligand, resn HEM

# Select the Iron atom specifically
select iron, name FE

# Select residues within 4.0 Angstroms of the ligand (excluding the ligand itself)
select close_residues, (byres (ligand around 4.0)) & ! ligand

# Show the environment
hide everything, all
bg_color white
# Do not show double bonds:
set valence, 0
show sticks, close_residues
show sticks, ligand
color atomic, close_residues
color red, ligand
```

- **&** = Logical AND
- **!** = Logical NOT

Now display in the context of the protein backbone:
```
show cartoon, 1mbo
color gray80, 1mbo
color atomic, close_residues
color red, ligand
```

---

## **Step 4: Surfaces and Hydrophobicity**

Visualizing the "skin" of the protein helps identify binding pockets.

```pymol
# Show the molecular surface
hide everything, all
show surface, 1mbo

# Make it semi-transparent to see the internal structure
set transparency, 0.5

# Color by hydrophobicity
color gray80, 1mbo
select hydrophobic, resn ALA+VAL+LEU+ILE+PHE+TRP+MET
color orange, hydrophobic

# add the cartoon model, duplicate for separate color assignment
create cartoon_object, 1mbo
hide everything, cartoon_object
show cartoon, cartoon_object
color deepteal, cartoon_object

# Sdd the ligand
show sticks, ligand
color purple, ligand
```

---

## **Step 5: Vacuum Electrostatics**

Identify how charge is distributed on the protein surface.

1. Go to **Action (A) > generate > vacuum electrostatics > protein contact potential**.
2. Identify the **heme pocket**. 
3. **Task:** Is the pocket positively (blue) or negatively (red) charged? How does this match the ligand's properties?

---

### Summary

1. **3D navigation** in the PyMOL viewport.
2. Use **Boolean operators** (`&`, `!`) for complex selections.
3. Visualize **molecular surfaces** and adjust **transparency**.
4. Map **chemical properties** (hydrophobicity, charge) onto structural models.

---

[[PyMOL/1_pdb_intro\|← Previous]] \| [[PyMOL/3_figures_contacts\|Next →]]
