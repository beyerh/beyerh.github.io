---
{"dg-publish":true,"permalink":"/py-mol/4-styling-mutagenesis/","title":"Exercise 4: Visualizing and Mutating Myoglobin"}
---

# PyMOL Exercise: Visualizing and Mutating Myoglobin (1MBO) with Heme Environment

This tutorial guides you step-by-step through **visualizing the heme environment of Myoglobin (PDB: 1MBO)**, selectively displaying key side chains, and performing a **residue mutation** (His64 → Ala) using PyMOL. We'll also use a community **styling script** for visualization.

---

## **Step 0: Prepare the Styling Script**

Download a community PyMOL styling script, e.g., [`pymol_style.py`](https://gist.github.com/kate-fie/50a749e03e81d15c320f0306150d6f66).  

1. Save the file locally, e.g., `~/pymol_style.py` or in your project folder.
2. We will use this script to apply **publication-ready colors, labels, and surface styles**.

---

## **Step 1: Load the Myoglobin Structure**

```pymol
# We start from scratch and fetch 1MBO from the PDB
reinitialize
fetch 1mbo

# Center and zoom on the protein
zoom all
hide everything, all
show cartoon, 1mbo
```

---

## **Step 2: Apply Professional Styling Script**

```pymol
# Load the styling script
run ~/pymol_style.py

# Apply general styling
setPretty
```

- This script sets **cartoon smoothing, ambient lighting, color palette, and label defaults**.

---

## **Step 3: Show Overall Structure**

```pymol
# Show cartoon for protein backbone
show cartoon, all
color white, all

# Show Heme as sticks
show sticks, resn HEM
color orange, resn HEM

# Set white background for publication look
bg_color white
```

---

## **Step 4: Select and Display the Heme Environment**

We want a **professional look**, so we only display:

- Heme
- Side chains within 5 Å of heme
- Key active site residues (His64, His93)

```pymol
# Select heme
select heme, resn HEM

# Select residues within 5 Å of heme
select heme_env, br. (byres heme around 5)

# Include distal (His64) and proximal (His93) histidines
select key_his, resi 64+93

# Combine selections
select display_env, heme_env or key_his

# Show only relevant environment
hide everything, all
show cartoon, 1mbo
show sticks, display_env
set valence, 0

# Show the heme ligand
show sticks, heme

# Color coding
color white, 1mbo
color lightpink, heme
color atomic, (heme and not elem C)
color marine, display_env
color magenta, resi 64  # distal His
color yellow, resi 93   # proximal His
```

---

## **Step 5: Label Key Residues Selectively**

```pymol
# Only label alpha carbons (or a single atom) of the histidines
label resi 64 and name CA, "His64 (distal)"
label resi 93 and name CA, "His93 (proximal)"

# Customize label appearance
set label_size, 18
set label_color, black
```

- By labeling **CA atoms only**, we avoid clutter from labeling all atoms.

---

## **Step 6: Zoom and Focus**

```pymol
# Zoom tightly around the selected environment and hide the cartoon
zoom display_env, 6
hide cartoon, 1mbo
```

- We **show only the relevant environment**, giving a clean, professional view.

---

## **Step 7: Perform the Mutation (His64 → Ala)**


1. Go to `Wizard → Mutagenesis`.
2. Select **His64**.
3. Choose **Ala** as new residue.
4. Preview rotamers and click **Apply**.

---

## **Step 8: Style and Render the Mutant**

```pymol
# Show sticks for Ala64
show sticks, resi 64
color red, resi 64
label resi 64 and name CA, "Ala64 (mutant)"

# Keep Heme visible
show sticks, resn HEM
color orange, resn HEM

# Set surface and transparency for environment
show surface, display_env
set transparency, 0.2, display_env

# Ray trace for publication-quality image
set ray_trace_mode, 1
set ray_shadows, 1
set antialias, 2
ray
```

---

## **Optional: Measure Distances for Context**

```pymol
# Distance from distal histidine to heme iron
distance dist_to_fe, resi 64 and name NE2, resn HEM and name FE

# Distance from proximal histidine to heme iron
distance prox_to_fe, resi 93 and name NE2, resn HEM and name FE
```

- Shows **coordination geometry** of active site residues.

---

## **Step 9: Save Session**

```pymol
# Save your PyMOL session for later
save 1MBO_mutation.pse
```

---

### Summary

1. Understand the **heme** environment in Myoglobin.
2. Selectively display only relevant residues and side chains.
3. Practice **mutating residues** while maintaining a clean visualization.
4. Apply **styling** with a reusable script.
5. Generate **publication-ready images**.

---

[[PyMOL/3_figures_contacts\|← Previous]] \| [[PyMOL/5_mcherry_intein\|Next →]]