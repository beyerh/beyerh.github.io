---
{"dg-publish":true,"permalink":"/py-mol/5-mcherry-intein/","title":"Exercise 5: Modeling mCherry and Intein Splicing"}
---

# PyMOL Exercise 4: Modeling mCherry and Intein Splicing

This exercise combines experimental structural data with AI-based modeling (AlphaFold3). You will explore the structure of **mCherry**, a fluorescent protein, and model the insertion of the ***Npu*DnaE intein** used in the course.

---

## **Step 1: Explore the mCherry Chromophore**

1. Search for **mCherry** on the PDB and fetch a structure.
2. Identify the **chromophore** (often labeled as `CH6` or similar HETATM).

```pymol
# Select and visualize the chromophore
select chromophore, resn CH6
show sticks, chromophore
zoom chromophore, 8
```

---

## **Step 2: modeling Intein Insertion with AlphaFold3**

In the laboratory course, you used the ***Npu*DnaE intein** inserted into **mCherry**.

1. Retrieve the amino acid sequence of your **mCherry-intein construct** (e.g., from Benchling).
2. Go to the [AlphaFold3 Server](https://alphafoldserver.com/) and run a structure prediction using the sequence of mCherry with intein insertion.
3. Download the resulting `.cif` model.

---

## **Step 3: Analyze the Model in PyMOL**

Load your AlphaFold model and compare it to the experimental templates.

```pymol
# Load your AF model
load your_model_af3.pdb, my_model

# Color the model by modelling confidence (pLDDT)
# Note: Requires a script like coloraf.py or a manual spectrum
spectrum b, blue_white_red, my_model, minimum=50, maximum=90

# Or better using a script:
run https://raw.githubusercontent.com/cbalbin-bio/pymol-color-alphafold/master/coloraf.py

coloraf my_model
```

- **plDDT Score:** High confidence (>90) is blue, low confidence (<50) is red. Which parts of your model are flexible?

---

## **Step 4: Measure Distances and Superimpose Structures**

1. **Catalytic Residues:** Identify the residues involved in protein splicing at the junctions and highlight them as colored sticks.
2. **Measure:** Use **Wizard** > **Measuremet** to check the proximity of the nucleophilic atoms.
3. **Superposition:** Align the AF model to the original mCherry structure.

```pymol
# Align the AF model to the native mCherry or use the (A)ction button
align my_model, 2H5Q
```

Inspect the fluorophore region. Did AlphaFold model it correctly?

---

## **Step 5: Challenge - Design a New Intein Insertion**

Use AlphaFold3 to generate a protein structure model with the *Npu*DnaE intein inserted. Retrieve the *Npu*DnaE intein sequence from Benchling and insert it into any of the proteins below (or choose your own target). Choose an appropriate insertion site and modify it if needed (remember the +1 residue insertion site). You can also look for insertion sites in the literature, but here, it is just about practice.

- *Streptococcus pyogenes* Cas9 nuclease
- T7 RNA Polymerase
- Bacillus amyloliquifaciens Barnase
- Human Caspase-3
- An aminoacyl tRNA synthetase (with or without tRNA), e.g. a human asparaginyl-tRNA synthetase
- *Providencia stuartii Pst*I restriction enzyme

**Goal:** Choose a site that likely breaks the protein function when the intein is present, but allows it to restore function after splicing.

---

### Summary

1. Identify and visualize **post-translationally modified chromophores**.
2. Integrate **AI-predicted models** into the PyMOL workflow.
3. Interpret **confidence scores (pLDDT)** from AlphaFold.
4. Perform **structural superposition** to compare models and templates.
5. Apply structural knowledge to **protein engineering** (intein insertion).

---

[[PyMOL/4_styling_mutagenesis\|← Previous]] \| [[PyMOL/6_scripting\|Next →]]
