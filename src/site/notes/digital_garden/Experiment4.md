---
{"dg-publish":true,"permalink":"/digital-garden/experiment4/"}
---


# Experiment IV: Intein-Catalyzed Protein Domain Swapping at the Plasma Membrane

**Supervisors:** Cha San Koh, Daniel Wiebensohn, Hannes Beyer

This experiment aims to induce either the addition or exchange of two protein domains at the plasma membrane of mammalian HeLa cells using split intein technology. Here, the construct design determines whether an intein *trans*-splicing reaction yields one of the two possible outcomes. To determine the localization of the two proteins, we will use the green fluorescent protein GFP and the red fluorescent protein mCherry, allowing for their analysis via confocal fluorescence microscopy (**Figure 18**). Both fluorescent proteins are genetically fused to one half of the DnaE intein from *Nostoc punctiforme* (*Npu*DnaE intein split fragments, abbreviated as IntN and IntC for the N- and C-terminal fragment, respectively), which you also used in Experiment III. GFP is additionally fused to an N-terminal myristylation/palmitylation signal derived from the Src kinase Lck, leading to cotranslational myristoylation at glycine residue 2 and then posttranslational palmitoylation at cysteine residues 3 and 5 (Akimzhanov and Boehning, 2015). Modification with these fatty acids leads to the attachment of the protein to inner cell membranes.

In the experiment, you will transiently transfect human HeLa cells with different combinations of the following plasmids encoding two versions of the membrane-attached GFP protein fused to IntN, or cytosolic mCherry fused to IntC. While we expect GFP to localize at the membrane and mCherry in the cytosol when transfected into cells, their cotransfection should induce the protein splicing reaction, which we will observe by confocal microscopy.

![Figure 18. \*\* Split intein-catalyzed protein trans-splicing (PTS) reaction either leading to the addition (left), or exchange (right) of GFP and mCherry at the plasma membrane, depending on the domain order of the GFP constructs (pDD130 vs pDD132). The IntC-fused mCherry construct pDD131 is identical in both approaches.](/img/user/figures/inteins_plasms_membrane.png)

**Figure 18.** \*\* Split intein-catalyzed protein trans-splicing (PTS) reaction either leading to the addition (left), or exchange (right) of GFP and mCherry at the plasma membrane, depending on the domain order of the GFP constructs (pDD130 vs pDD132). The IntC-fused mCherry construct pDD131 is identical in both approaches.

In cells, many relevant signaling pathways initiate or pass through microdomains at the plasma membrane, often linking the perception of extracellular signals via membrane integral receptors to the cytosol. Therefore, modulating the localization of proteins involved in cell signaling represents an important tool to regulate cellular behavior. However, the induction of protein domain swapping might likewise be employed to regulate diverse cellular mechanisms, for example, by exchanging antagonistically functional protein domains, such as activators and repressors.

### Materials

**Table 15.** Materials used in Experiment III.

| Item                        | Composition/Concentration                                      | Application                           |
|:----------------------------|:---------------------------------------------------------------|:--------------------------------------|
| Arabinose                   | 20%                                                            | Induce expression of $P_{\text{BAD}}$ |
| Ampicillin                  | 100 mg/mL                                                      | Selection marker                      |
| Kanamycin                   | 50 mg/mL                                                       | Selection marker                      |
| IPTG                        | 1 M                                                            | Induce expression of $P_{\text{T7}}$  |
| LB-Medium                   | 10 g/L tryptone, 5g/L yeast extract, 10 g/L NaCl, pH 7.0.      | Bacteria growth medium                |
| PBS                         | 2.7 mM KCl, 1.5 mM KH₂PO₄, 8.0 mM Na₂HPO₄, 137 mM NaCl in dH₂O | Buffer used for cell diluting         |
| *E. coli* T7 express strain |                                                                | Expresses T7 RNA- polymerase          |

**Table 16.** Plasmid DNA (Minipreps)

| Name   | Description                | Concentration |
|--------|----------------------------|---------------|
| pDD130 | PSV40-LckM/P-GFP-Int~N~-pA | 100 ng/µL     |
| pDD131 | PSV40-Int~C~-mCherry-pA    | 100 ng/µL     |
| pDD132 | PSV40-LckM/P-Int~N~-GFP-pA | 100 ng/µL     |

**Table 17.** Media

| Name                 | Description/Composition                                                                                                                   |
|----------------------|-------------------------------------------------------------------------------------------------------------------------------------------|
| DMEMcomplete         | Dulbecco’s Modified Eagle Medium (Gibco), 10% fetal bovine serum (FBS, PAN-Biotech), 100 U/mL penicillin, 0.1 mg/mL streptomycin (Gibco). |
| Opti-MEMTM           | Optimized minimum essential medium (Gibco), serum-free.                                                                                   |
| Lysogeny broth (LB)  | 10 g/L tryptone, 5g/L yeast extract, 10 g/L NaCl, pH 7.0.                                                                                 |
| LB-agar plates (Amp) | 20 g/L Bacto Agar in 500 mL dH~2~O, 100 µg/mL Ampicillin.                                                                                 |

**Table 18.** Cells

| Name            | Description                                                                                                                                                                    |
|-----------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| HeLa            | *H. sapiens* cervix carcinoma derivative, epithelial-like, (ACC 57, DSMZ).                                                                                                     |
| *E. coli* TOP10 | Chemically-competent cells. Genotyp: F-*mcrA* Δ(*mrr-hsd\_RMS-*mcr\_BC) Φ80*Lac*ZΔM15 Δ*Lac*X74 *rec*A1 *ara*D139 Δ(*araleu*) 7697 *gal*U *gal*K *rps*L (StrR) *end*A1 *nup*G. |

**Table 19.** Buffers and chemicals

| Name                    | Description/Concentration                                                                        |
|-------------------------|--------------------------------------------------------------------------------------------------|
| PBS                     | 2.7 mM KCl, 1.5 mM KH<sub>2</sub>PO4, 8.0 mM Na<sub>2</sub>HPO4, 137 mM NaCl in dH<sub>2</sub>O. |
| Trypsin/EDTA in PBS     | 0.05% Trypsin/ 0.02% EDTA in PBS; PAN Biotech Cat. No. P10-023500                                |
| RES/P1                  | 50 mM Tris-HCl, 10 mM EDTA, 100 μg/mL RNase A, dH<sub>2</sub>O to 1 L.                           |
| LYS/P2                  | 0.2 M NaOH, 1% SDS, dH<sub>2</sub>O to 1 L.                                                      |
| NEU/P3                  | 3.0 M potassium acetate, dH~2~O to 1 L.                                                          |
| EQU                     | 750 mM NaCl, 50 mM MOPS, 15% isopropanol, 0,15% Triton X-100, dH<sub>2</sub>O to 1 L.            |
| WASH                    | 1.0M NaCl, 50 mM MOPS, 15% isopropanol, dH~2~O to 1 L.                                           |
| ELU                     | 1.25M NaCl, 50 mM Tris-Cl, 15% isopropanol, dH~2~O to 1 L.                                       |
| 2-Propanol              | (Sigma)                                                                                          |
| 70% Ethanol             | 70 ml Ethanol absolute (Chemsolute), dH~2~O to 100 mL.                                           |
| H~2~O                   |                                                                                                  |
| Polyethyleneimine (PEI) | 1 mg/mL PEI (25 kDa) in dH~2~O, pH 7 (HCl), sterile filtered with 0.2 μM pore size.              |
| Mowiol (Roth)           | 6 g glycerol, 2.4 g Mowiol 4-88, 6 mL dH~2~O, 12 mL 0.2 M Tris-HCl pH 8.5.                       |
| DABCO (Roth)            | 1,4-diazabicyclo\[2.2.2\]octane (anti-photobleaching reagent).                                   |

**Table 20.** Consumables

| Name           | Description                                                           |
|----------------|-----------------------------------------------------------------------|
| Midi Columns   | NucleoBond Xtra Midi Kit; Macherey-Nagel REF. 740410<br>              |
| 24-well plates | Costar® 24-well Clear TC-treated Multiple Well Plates, cat. No. 3524. |

### Protocol

#### Day 7: Plasmid Transformation

Each participant will transform one plasmid into *E. coli* TOP10 cells, inoculate a culture on day 4, and perform a plasmid midiprep on day 5.

The different plasmids are distributed as follows:

**Odd group numbers:** pDD130 and pDD131

**Even group numbers:** pDD131 and pDD132

Please refer to Experiment I for the transformation protocol. Use 1 µL of the provided plasmid DNA per transformation into one tube of competent *E. coli* TOP10 cells. Spread 50 µL of culture on one LB-Amp plate (asymmetrically, you want to be able to pick a single colony the next day). Incubate the plate overnight at 37°C.

#### Day 8: Culture Inoculation

1.  Add 100 µL of Ampicillin to one Erlenmeyer flask containing 100 mL LB medium.
2.  Using a sterile 200 µL pipette tip, pick one colony from your transformation on day 7 and inoculate the medium.
3.  Shake the flask overnight at 37°C, shaking at 180 rpm.

#### Day 9: Culture Harvesting

1.  Harvest 100 mL culture by centrifugation for 5 min at 5,000 *xg* at RT in a 50 mL Falcon tube.
2.  Remove the supernatant (SN).
3.  Store at -20°C

#### Day 10: Plasmid Midiprep

1.  Add 8 mL of buffer RES supplemented with RNAase (M. Nagel, 60 µg mL-1) to the Falcon tube, thoroughly resuspend the cells.
2.  Add 8 mL lysis buffer LYS (if you notice precipitated SDS, warm it first until it dissolves). Mix by inverting 6 to 8 times. DO NOT VORTEX.
3.  Incubate 5 min at RT.
4.  Add 8 mL neutralization buffer NEU. Mix immediately by inverting the tube 6 to 8 times. DO NOT VORTEX.
5.  Centrifuge 10 min, 12,000 *xg* at RT. (Afterwards, set the centrifuge to 4°C for a later step)
6.  Meanwhile, equilibrate the column/filter with 10 mL equilibration buffer EQU (apply the buffer onto the rim of the column filter, not the center), and allow the column to drain by gravity flow.
7.  Load supernatant on the filter/column, and allow the column to drain by gravity flow.
8.  Add 10 mL equilibration buffer EQU for the 1st wash (on the rim of the filter).
9.  Discard the column filter.
10. Add 10 mL of wash buffer WASH for the 2nd wash (directly on the middle of the column).
11. Place a 15 mL Falcon tube under the column and elute the DNA with 5 mL elution buffer ELU.
12. Add 3.5 mL of isopropanol to the eluate. Vortex thoroughly.
13. Centrifuge 30 min, 12,000 *xg* at 4°C. (Afterwards, set the centrifuge to RT for the next step).
14. Discard SN by decanting (Be careful at this step. You should see a small white DNA pellet, which you do not want to lose). Show the pellet to your supervisor to discuss in what volume you should resuspend the pellet in the last step.
15. Wash the DNA pellet with 2 mL 70% EtOH.
16. Centrifuge 5 min, 12,000 *xg* at RT.
17. Carefully discard the SN using the pipette. The pellet is usually very loose at this step.
18. Air-dry the pellet (a few hours at RT, or in the oven at 58°C for approx. 20 min).
19. Resuspend with 70–120 µL ddH$_2$O (sterile).
20. Incubate 30 min at 37°C, resuspend by gentle pipetting.
21. Dilute the DNA 1:10 and determine the concentration using the nanodrop (eventually adjust the concentration to 2 µg µL⁻¹).
22. Freeze the extracted plasmids

#### Day 11: Seeding HeLa Cells on Glass Coverslips

This step should be performed only by one member of each group in order to prevent overcrowding in the cell culture room. Together with the supervisors, you will prepare a shared cell suspension. Each present group member will then seed the required number of cells in a 24-well plate (one plate per group)

1.  Prepare a 15 mL Falcon tube containing 8 mL prewarmed DMEMcomplete medium.
2.  Remove supernatant (pump).
3.  Add 2 mL Trypsin and incubate the plate for 5 min at 37°C.
4.  Detach and resuspend the cells using a 1000 µL pipette. Transfer the suspension to the prepared medium. (The serum in the medium will inactivate the Trypsin).
5.  Centrifuge cells for 3 min, 300 *xg*
6.  Remove supernatant and resuspend the cell pellet with 10 mL fresh medium.
7.  Prepare a Countess 3 counting chamber.
8.  Add 14 µL of the cell suspension to the cup.
9.  Count cells using the Countess 3.
10. The Countess 3 provides information on the concentration (cells/mL) and viability (in %) of the cells. Please record this information for your protocol.
11. Determine the number of cells: counted cells/mL \* 10 mL (volume) = total cells. The number provided by the Countess 3 for the cell concentration corresponds to *µ1*.
12. Seed HeLa cells as follows:

- Prepare a cell suspension with a concentration of 60,000 cells/mL (-&gt; *c2)* by dilution with DMEMcomplete medium. Prepare 30 mL (-&gt; *v2)* of cell suspension in order to have enough for all groups. Use a 50 mL Falcon tube. The required dilution volume *v1* can be calculated according to the formula *c1* \* *v1* = *c2* \* *v2*.
- Seed 500 µL of cell suspension (containing 30,000 HeLa cells) into each well of a 24-well plate containing a glass cover slip (prepared by supervisors in advance). Each group should seed 6 wells into an individual plate.

> *Well plate layout: Seed wells 1, 2, and 3 in a 24-well plate (6 wells per group).*

1.  Place the cell culture plate into the 37°C incubator to allow them to attach to the glass coverslip for the PEI transfection on day 12.

#### Day 12: PEI Transfection

1.  Per well, dilute 0.75 µg of DNA in OptiMEM to a final volume of 50 µL (remember your Midi-prep concentration). Please check **Table 21** and **Table 22** for further information.
2.  When transfecting multiple plasmids for the same setup, divide the total DNA amount (0.75 µg) by the number of plasmids which are transfected (equal plasmid load). Note: keep ca. 0.75 µg as total DNA amount; the ratio of DNA: PEI is important for the transfection efficiency!
3.  Per well, dilute 2.5 µL of PEI solution in OptiMEM to a final volume of 50 µL. Vortex. Please check **Table 21** and **Table 22** for further information.
4.  Add an equal volume of PEI solution to the DNA solution.
5.  Vortex the solution immediately and thoroughly for 10 s. Complexation of PEI with DNA, into small particles able to enter the cell during transfection, is dependent on thorough mixing at this step.
6.  Incubate for 15 min at RT.
7.  Per well, add the premixed 100 µL PEI/DNA mix drop-wise to each well. DO NOT VORTEX!
8.  Incubate for 4 h at 37°C in the cell culture incubator.
9.  Exchange medium for fresh cultivation medium (500 µL per well).

**Table 21.** Transfection Set up 1 for odd group numbers.

| Setup   | Plasmid         | Amount  | DNA conc. | µL/well      | µL total |
|---------|-----------------|---------|-----------|--------------|----------|
| Setup 1 | pDD130          | 1       | Enter C   | 0.75/C = V   | V×3      |
| \-      | OptiMEM         | \-      | \-        | 50-V = O     | O×3      |
| Setup 2 | pDD131          | 1       | Enter C   | 0.75/C = V   | V×3      |
| \-      | OptiMEM         | \-      | \-        | 50-V = O     | O×3      |
| Setup 3 | pDD130 + pDD131 | 1 each  | Enter C   | 0.375/C = V  | V×3      |
| \-      | OptiMEM         | \-      | \-        | 50-V1-V2 = O | O×3      |
| PEI Mix | PEI             | 8 wells | \-        | 2.5 µL       | 20 µL    |
| \-      | OptiMEM         | 8 wells | \-        | 47.5 µL      | 380 µL   |

**Table 22.** Transfection Set up 1 for even group numbers.

| Setup   | Plasmid         | Amount  | DNA conc. | µL/well      | µL total |
|---------|-----------------|---------|-----------|--------------|----------|
| Setup 1 | pDD131          | 1       | Enter C   | 0.75/C = V   | V×3      |
| \-      | OptiMEM         | \-      | \-        | 50-V = O     | O×3      |
| Setup 2 | pDD132          | 1       | Enter C   | 0.75/C = V   | V×3      |
| \-      | OptiMEM         | \-      | \-        | 50-V = O     | O×3      |
| Setup 3 | pDD131 + pDD132 | 1 each  | Enter C   | 0.375/C = V  | V×3      |
| \-      | OptiMEM         | \-      | \-        | 50-V1-V2 = O | O×3      |
| PEI Mix | PEI             | 8 wells | \-        | 2.5 µL       | 20 µL    |
| \-      | OptiMEM         | 8 wells | \-        | 47.5 µL      | 380 µL   |

#### Day 13: Paraformaldehyde (PFA) Fixation of Cells for Confocal Microscopy

1.  Wash cells with 500 µL PBS once.
2.  Overlay cells with 200 µL 4% PFA, incubate on ice for 10 min, followed by an additional 10 min at RT.
3.  Remove PFA (NOTE: used tips and liquid waste go to special waste containers!).
4.  Add 400 µL of PBS.
5.  Prepare and label object slides.
6.  Add 8 µL of prepared Mowiol with DABCO on the object slides (supervisors will demonstrate how to do it).
7.  Be careful not to pipette any air bubbles.
8.  Carefully take out coverslips from the 24-well plate using tweezers.
9.  Carefully get rid of water droplets with the help of fine tissue.
10. Place the coverslips with the cells facing down onto the Mowiol droplet. Avoid air bubbles.
11. Dry slides at 37°C for 30 min.

#### Confocal Microscopy

One pair of odd and even group members proceeds to the confocal microscope at a time, accompanied by their supervisors. Afterwards, you may analyze the data using FIJI in the seminar room.


---
[[digital_garden/Experiment3\|< Previous: Experiment III]] | [[digital_garden/Experiment5\|Next: Experiment V >]]
