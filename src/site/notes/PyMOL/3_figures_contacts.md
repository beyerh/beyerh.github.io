---
{"dg-publish":true,"permalink":"/py-mol/3-figures-contacts/","title":"Exercise 3: Annotation, Polar Contacts, Figures"}
---

# PyMOL Exercise 3: Annotation, Polar Contacts, and Figures

This exercise focuses on preparing figures. You will learn how to label atoms, identify hydrogen bonds, and use high-quality rendering (ray tracing).

---

## **Step 1: Annotation and Labeling**

Labels are essential for communicating specific details in a structure. Visualize the ligand in `1mbo` and then add annotations as follows:

```pymol
# Label the iron atom in 1MBO
label iron, "Fe2+"

# Customize label appearance
set label_size, 20
set label_font_id, 7   # Bold font
set label_color, red

# To hide labels again
hide labels, all
```

---

## **Step 2: Visualize Polar Contacts**

Polar contacts (hydrogen bonds and salt bridges) are important forces that stabilize structures.

1. Ensure you have the `1mbo` cartoon and the **heme** sticks visible.
2. Go to **Action (A) > find > polar contacts > excluding solvent**.
3. **Task:** Observe the dashed lines. Which residues in the protein are interacting with the heme group?

---

## **Step 3: High-Quality Rendering**

The standard view in PyMOL is optimized for speed. For a publication-quality image, use the **Ray** command.

```pymol
# Prepare the scene
orient
zoom 1mbo, 2

# Set quality parameters
set antialias, 2                   # Smooth edges
set ray_opaque_background, off     # Transparent background
set ray_shadows, on                # Add depth with shadows
set ambient, 0.2                   # Soften lighting
set specular, off                  # Remove "plastic" highlights

# Render the image (e.g., 1200x900 pixels)
ray 1200, 900                      # Or better use the Draw/Ray button
```

- After ray tracing, use the **Draw/Ray** button menu to **Save Image as PNG**.

---

## **Step 4: Advanced Rendering Modes**

PyMOL has special modes to make secondary structure "pop".

```pymol
# Black outline mode (good for cartoons)
set ray_trace_mode, 1
ray
```

---

### Summary

1. Add and customize **text labels** in 3D space.
2. Automatically identify and display **polar contacts**.
3. Configure **lighting and shadow settings** for better depth.
4. Generate and export **high-resolution images** using Ray tracing.

---

[[PyMOL/2_pymol_basics\|← Previous]] \| [[PyMOL/4_styling_mutagenesis\|Next →]]
