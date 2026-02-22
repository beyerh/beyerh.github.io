---
{"dg-publish":true,"permalink":"/garden-06-experiment4/","title":"Experiment 4: Protein Splicing HeLa"}
---

## Experiment IV: Intein-Catalyzed Protein Domain Swapping at the Plasma Membrane

**Supervisors:** Cha San Koh, Daniel Wiebensohn, Hannes Beyer

This experiment aims to induce either the addition or exchange of two protein domains at the plasma membrane of mammalian HeLa cells using split intein technology. Here, the construct design determines whether an intein *trans*-splicing reaction yields one of the two possible outcomes. To determine the localization of the two proteins, we will use the green fluorescent protein GFP and the red fluorescent protein mCherry, allowing for their analysis *via* confocal fluorescence microscopy (**Figure 1**). Both fluorescent proteins are genetically fused to one half of the DnaE intein from *Nostoc punctiforme* (*Npu*DnaE intein split fragments, abbreviated as Int<sub>N</sub> and Int<sub>C</sub> for the N- and C-terminal fragment, respectively), which you also used in Experiment III. GFP is additionally fused to an N-terminal myristylation/palmitylation signal derived from the Src kinase Lck, leading to cotranslational myristoylation at glycine residue 2 and then posttranslational palmitoylation at cysteine residues 3 and 5 (Akimzhanov and Boehning, 2015). Modification with these fatty acids leads to the attachment of the protein to inner cell membranes.

In the experiment, you will transiently transfect human HeLa cells with different combinations of the following plasmids encoding two versions of the membrane-attached GFP protein fused to Int<sub>N</sub>, or cytosolic mCherry fused to Int<sub>C&lt;/su<sub></sub>b&gt;. While we expect GFP to localize at the membrane and mCherry in the cytosol when transfected into cells, their cotransfection should induce the protein splicing reaction, which we will observe by confocal microscopy.

<figure id="fig:domain-swapping" class="align-left" style="width: 100%; display: block; margin-right: auto">

![Figure 1](/img/user/figures/inteins_plasms_membrane.png)

<figcaption>
<strong>Figure 1.</strong> 
<strong>Split intein-catalyzed protein trans-splicing (PTS)</strong>
reaction either leading to the addition (left), or exchange (right) of
GFP and mCherry at the plasma membrane, depending on the domain order of
the GFP constructs (pDD130 vs pDD132). The Int<sub>C</sub>-fused mCherry
construct pDD131 is identical in both approaches.
</figcaption>
</figure>

In cells, many relevant signaling pathways initiate or pass through microdomains at the plasma membrane, often linking the perception of extracellular signals *via* membrane integral receptors to the cytosol. Therefore, modulating the localization of proteins involved in cell signaling represents an important tool to regulate cellular behavior. However, the induction of protein domain swapping might likewise be employed to regulate diverse cellular mechanisms, for example, by exchanging antagonistically functional protein domains, such as activators and repressors.

### Materials

test

### Protocol

#### Day 7: Plasmid Transformation

Each participant will transform one plasmid into *E. coli* TOP10 cells, inoculate a culture on day 8, and perform a plasmid midiprep on day 10.

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
18. Air-dry the pellet (a few hours at RT, or in the oven at 60°C for approx. 20 min).
19. Resuspend with 70–120 µL ddH$_2$O (sterile).
20. Incubate 30 min at 37°C, resuspend by gentle pipetting.
21. Dilute the DNA 1:10 and determine the concentration using the nanodrop (eventually adjust the concentration to 2 µg/µL).
22. Freeze the extracted plasmids.

#### Day 11: Seeding HeLa Cells on Glass Coverslips

This step should be performed only by one member of each group in order to prevent overcrowding in the cell culture room. Together with the supervisors, you will prepare a shared cell suspension. Each present group member will then seed the required number of cells in a 24-well plate (one plate per group)

1.  Prepare a 15 mL Falcon tube containing 8 mL prewarmed DMEMcomplete medium.
2.  Remove supernatant (pump).
3.  Add 2 mL Trypsin and incubate the plate for 5 min at 37°C.
4.  Detach and resuspend the cells using a 1000 µL pipette. Transfer the suspension to the prepared medium. (The serum in the medium will inactivate the Trypsin).
5.  Centrifuge cells for 3 min, 300 *xg*.
6.  Remove supernatant and resuspend the cell pellet with 10 mL fresh medium.
7.  Prepare a Countess 3 counting chamber.
8.  Add 14 µL of the cell suspension to the cup.
9.  Count cells using the Countess 3.
10. The Countess 3 provides information on the concentration (cells/mL) and viability (in %) of the cells. Please record this information for your protocol.
11. Determine the number of cells: counted cells/mL \* 10 mL (volume) = total cells.
12. Seed HeLa cells as follows:

- Prepare a cell suspension with a concentration of 60,000 cells/mL (→ *c2)* by dilution with DMEMcomplete medium. Prepare 35 mL (→ *v2)* of cell suspension in order to have enough for all groups. Use a 50 mL Falcon tube. The required dilution volume *v1* can be calculated according to the formula *c1* \* *v1* = *c2* \* *v2*.
- Seed 500 µL of cell suspension (containing 30,000 HeLa cells) into each well of a 24-well plate **containing a glass cover slip** (prepared by supervisors in advance). Each group should seed 6 wells into an individual plate.

<figure id="tbl:yourtablelabel" class="align-center" style="width: 30%; display: block; margin-left: auto; margin-right: auto">
  <figcaption>
    <strong>Table 7.</strong> 
Well plate layout: Seed wells 1, 2, and 3 in a 24-well plate (6 wells
per group).
  </figcaption>
<table>
<colgroup>
<col style="width: 10%" />
<col style="width: 15%" />
<col style="width: 15%" />
<col style="width: 15%" />
<col style="width: 15%" />
<col style="width: 15%" />
<col style="width: 15%" />
</colgroup>
<thead>
<tr>
<th></th>
<th>1</th>
<th>2</th>
<th>3</th>
<th>4</th>
<th>5</th>
<th>6</th>
</tr>
</thead>
<tbody>
<tr>
<td>A</td>
<td>x</td>
<td>x</td>
<td>x</td>
<td></td>
<td></td>
<td></td>
</tr>
<tr>
<td>B</td>
<td>x</td>
<td>x</td>
<td>x</td>
<td></td>
<td></td>
<td></td>
</tr>
<tr>
<td>C</td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
</tr>
<tr>
<td>D</td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
</tr>
</tbody>
</table>
</figure>

1.  Place the cell culture plate into the 37°C incubator to allow them to attach to the glass coverslip for the PEI transfection on day 12.

#### Day 12: PEI Transfection

1.  Per well, dilute 0.75 µg of DNA in OptiMEM to a final volume of 50 µL (remember your Midi-prep concentration). Please check **Table 8** and **Table 9** for further information.
2.  When transfecting multiple plasmids for the same setup, divide the total DNA amount (0.75 µg) by the number of plasmids which are transfected (equal plasmid load). Note: keep ca. 0.75 µg as total DNA amount; the ratio of DNA: PEI is important for the transfection efficiency!
3.  Per well, dilute 2.5 µL of PEI solution in OptiMEM to a final volume of 50 µL. Vortex. Please check **Table 8** and **Table 9** for further information.
4.  Add an equal volume of PEI solution to the DNA solution.
5.  Vortex the solution immediately and thoroughly for 10 s. Complexation of PEI with DNA, into small particles able to enter the cell during transfection, is dependent on thorough mixing at this step.
6.  Incubate for 15 min at RT.
7.  Per well, add the premixed 100 µL PEI/DNA mix drop-wise to each well. DO NOT VORTEX!
8.  Incubate for 4 h at 37°C in the cell culture incubator.
9.  Exchange medium for fresh cultivation medium (500 µL per well).

<figure id="tbl:transfection-odd" class="align-left" style="width: 100%; float: left; margin-right: 1em">
  <figcaption>
    <strong>Table 8.</strong> 
Transfection Set up 1 for odd group numbers.
  </figcaption>
<table>
<thead>
<tr>
<th>Setup</th>
<th>Plasmid</th>
<th>Amount</th>
<th>DNA conc.</th>
<th>µL/well</th>
<th>µL total</th>
</tr>
</thead>
<tbody>
<tr>
<td>Setup 1</td>
<td>pDD130</td>
<td>1</td>
<td>Enter C</td>
<td>0.75/C = V</td>
<td>V×3</td>
</tr>
<tr>
<td>-</td>
<td>OptiMEM</td>
<td>-</td>
<td>-</td>
<td>50-V = O</td>
<td>O×3</td>
</tr>
<tr>
<td>Setup 2</td>
<td>pDD131</td>
<td>1</td>
<td>Enter C</td>
<td>0.75/C = V</td>
<td>V×3</td>
</tr>
<tr>
<td>-</td>
<td>OptiMEM</td>
<td>-</td>
<td>-</td>
<td>50-V = O</td>
<td>O×3</td>
</tr>
<tr>
<td>Setup 3</td>
<td>pDD130 + pDD131</td>
<td>1 each</td>
<td>Enter C</td>
<td>0.375/C = V</td>
<td>V×3</td>
</tr>
<tr>
<td>-</td>
<td>OptiMEM</td>
<td>-</td>
<td>-</td>
<td>50-V1-V2 = O</td>
<td>O×3</td>
</tr>
<tr>
<td>PEI Mix</td>
<td>PEI</td>
<td>8 wells</td>
<td>-</td>
<td>2.5 µL</td>
<td>20 µL</td>
</tr>
<tr>
<td>-</td>
<td>OptiMEM</td>
<td>8 wells</td>
<td>-</td>
<td>47.5 µL</td>
<td>380 µL</td>
</tr>
</tbody>
</table>
</figure>
<figure id="tbl:transfection-even" class="align-left" style="width: 100%; float: left; margin-right: 1em">
  <figcaption>
    <strong>Table 9.</strong> 
Transfection Set up 1 for even group numbers.
  </figcaption>
<table>
<thead>
<tr>
<th>Setup</th>
<th>Plasmid</th>
<th>Amount</th>
<th>DNA conc.</th>
<th>µL/well</th>
<th>µL total</th>
</tr>
</thead>
<tbody>
<tr>
<td>Setup 1</td>
<td>pDD131</td>
<td>1</td>
<td>Enter C</td>
<td>0.75/C = V</td>
<td>V×3</td>
</tr>
<tr>
<td>-</td>
<td>OptiMEM</td>
<td>-</td>
<td>-</td>
<td>50-V = O</td>
<td>O×3</td>
</tr>
<tr>
<td>Setup 2</td>
<td>pDD132</td>
<td>1</td>
<td>Enter C</td>
<td>0.75/C = V</td>
<td>V×3</td>
</tr>
<tr>
<td>-</td>
<td>OptiMEM</td>
<td>-</td>
<td>-</td>
<td>50-V = O</td>
<td>O×3</td>
</tr>
<tr>
<td>Setup 3</td>
<td>pDD131 + pDD132</td>
<td>1 each</td>
<td>Enter C</td>
<td>0.375/C = V</td>
<td>V×3</td>
</tr>
<tr>
<td>-</td>
<td>OptiMEM</td>
<td>-</td>
<td>-</td>
<td>50-V1-V2 = O</td>
<td>O×3</td>
</tr>
<tr>
<td>PEI Mix</td>
<td>PEI</td>
<td>8 wells</td>
<td>-</td>
<td>2.5 µL</td>
<td>20 µL</td>
</tr>
<tr>
<td>-</td>
<td>OptiMEM</td>
<td>8 wells</td>
<td>-</td>
<td>47.5 µL</td>
<td>380 µL</td>
</tr>
</tbody>
</table>
</figure>

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


----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------


\[\[garden\_05-Experiment3\|← Previous\]\] \| \[\[garden\_07-Experiment5\|Next →\]\]
