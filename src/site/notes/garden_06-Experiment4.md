---
{"dg-publish":true,"permalink":"/garden-06-experiment4/","title":"Experiment 4: Protein splicing domain swapping in HeLa cells"}
---


## Experiment IV: Intein-Catalyzed Protein Domain Swapping at the Plasma Membrane

**Supervisors:** Cha San Koh, Daniel Wiebensohn, Hannes Beyer

This experiment aims to induce either the addition or exchange of two protein domains at the plasma membrane of mammalian HeLa cells using split intein technology. Here, the construct design determines whether an intein *trans*-splicing reaction yields one of the two possible outcomes. To determine the localization of the two proteins, we will use the green fluorescent protein GFP and the red fluorescent protein mCherry, allowing for their analysis *via* confocal fluorescence microscopy (**[Figure 18](#fig:domain-swapping)**). Both fluorescent proteins are genetically fused to one half of the DnaE intein from *Nostoc punctiforme* (*Npu*DnaE intein split fragments, abbreviated as Int<sub>N</sub> and Int<sub>C</sub> for the N- and C-terminal fragment, respectively), which you also used in Experiment III. GFP is additionally fused to an N-terminal myristylation/palmitylation signal derived from the Src kinase Lck, leading to cotranslational myristoylation at glycine residue 2 and then posttranslational palmitoylation at cysteine residues 3 and 5 (Akimzhanov and Boehning, 2015). Modification with these fatty acids leads to the attachment of the protein to inner cell membranes.

In the experiment, you will transiently transfect human HeLa cells with different combinations of the following plasmids encoding two versions of the membrane-attached GFP protein fused to Int<sub>N</sub>, or cytosolic mCherry fused to Int<sub>C</sub>. While we expect GFP to localize at the membrane and mCherry in the cytosol when transfected into cells, their cotransfection should induce the protein splicing reaction, which we will observe by confocal microscopy.

<figure id="fig:domain-swapping" class="align-left" style="width: 100%; display: block; margin-right: auto">

![Figure 18](/img/user/figures/inteins_plasms_membrane.png)
<figcaption style="font-size: 0.9em; color: #555; margin-top: 0.5em; line-height: 1.5; font-style: normal; display: block;">

<strong style="color: #333;">Figure 18.</strong> <strong>Domain swapping at the plasma membrane.</strong> Split intein-catalyzed protein trans-splicing (PTS) reaction either leading to the addition (left), or exchange (right) of GFP and mCherry at the plasma membrane, depending on the domain order of the GFP constructs (pDD130 vs pDD132). The Int<sub>C</sub>-fused mCherry construct pDD131 is identical in both approaches.

</figcaption>

</figure>

In cells, many relevant signaling pathways initiate or pass through microdomains at the plasma membrane, often linking the perception of extracellular signals *via* membrane integral receptors to the cytosol. Therefore, modulating the localization of proteins involved in cell signaling represents an important tool to regulate cellular behavior. However, the induction of protein domain swapping might likewise be employed to regulate diverse cellular mechanisms, for example, by exchanging antagonistically functional protein domains, such as activators and repressors.

### Materials

<figure id="tbl:exp4materials" class="align-center" style="width: 100%; display: block; margin-left: auto; margin-right: auto">
  <figcaption style="font-size: 0.9em; color: #555; margin-bottom: 0.5em; line-height: 1.5; font-style: normal; display: block;">
    <strong style="color: #333;">Table 15.</strong> Materials used in Experiment IV.
  </figcaption>
<table>
<thead>
<tr>
<th style="text-align: left;">Item</th>
<th style="text-align: left;">Composition/Concentration</th>
<th style="text-align: left;">Application</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align: left;">Arabinose</td>
<td style="text-align: left;">20%</td>
<td style="text-align: left;">Induce expression of <span
class="math inline"><em>P</em><sub>BAD</sub></span></td>
</tr>
<tr>
<td style="text-align: left;">Ampicillin</td>
<td style="text-align: left;">100 mg/mL</td>
<td style="text-align: left;">Selection marker</td>
</tr>
<tr>
<td style="text-align: left;">Kanamycin</td>
<td style="text-align: left;">50 mg/mL</td>
<td style="text-align: left;">Selection marker</td>
</tr>
<tr>
<td style="text-align: left;">IPTG</td>
<td style="text-align: left;">1 M</td>
<td style="text-align: left;">Induce expression of <span
class="math inline"><em>P</em><sub>T7</sub></span></td>
</tr>
<tr>
<td style="text-align: left;">LB-Medium</td>
<td style="text-align: left;">10 g/L tryptone, 5 g/L yeast extract, 10
g/L NaCl, pH 7.0.</td>
<td style="text-align: left;">Bacteria growth medium</td>
</tr>
<tr>
<td style="text-align: left;">PBS</td>
<td style="text-align: left;">2.7 mM KCl, 1.5 mM KH₂PO₄, 8.0 mM Na₂HPO₄,
137 mM NaCl in dH₂O</td>
<td style="text-align: left;">Buffer used for cell diluting</td>
</tr>
<tr>
<td style="text-align: left;"><em>E. coli</em> T7 express strain</td>
<td style="text-align: left;"></td>
<td style="text-align: left;">Expresses T7 RNA- polymerase</td>
</tr>
</tbody>
</table>
</figure>

<figure id="tbl:exp3dna" class="align-left" style="width: 100%; float: left; margin-right: 1em">
  <figcaption style="font-size: 0.9em; color: #555; margin-bottom: 0.5em; line-height: 1.5; font-style: normal; display: block;">
    <strong style="color: #333;">Table 16.</strong> Plasmid DNA (Minipreps)
  </figcaption>
<table>
<thead>
<tr>
<th>Name</th>
<th>Description</th>
<th>Concentration</th>
</tr>
</thead>
<tbody>
<tr>
<td>pDD130</td>
<td>P<sub>SV40</sub>-LckM/P-GFP-Int<sub>N</sub>-pA</td>
<td>100 ng/µL</td>
</tr>
<tr>
<td>pDD131</td>
<td>P<sub>SV40</sub>-Int<sub>C</sub>-mCherry-pA</td>
<td>100 ng/µL</td>
</tr>
<tr>
<td>pDD132</td>
<td>P<sub>SV40</sub>-LckM/P-Int<sub>N</sub>-GFP-pA</td>
<td>100 ng/µL</td>
</tr>
</tbody>
</table>
</figure>

<figure id="tbl:exp3media" class="align-left" style="width: 100%; float: left; margin-right: 1em">
  <figcaption style="font-size: 0.9em; color: #555; margin-bottom: 0.5em; line-height: 1.5; font-style: normal; display: block;">
    <strong style="color: #333;">Table 17.</strong> Media
  </figcaption>
<table>
<thead>
<tr>
<th>Name</th>
<th>Description/Composition</th>
</tr>
</thead>
<tbody>
<tr>
<td>DMEMcomplete</td>
<td>Dulbecco’s Modified Eagle Medium (Gibco), 10% fetal bovine serum
(FBS, PAN-Biotech), 100 U/mL penicillin, 0.1 mg/mL streptomycin
(Gibco).</td>
</tr>
<tr>
<td>Opti-MEM<sup>TM</sup></td>
<td>Optimized minimum essential medium (Gibco), serum-free.</td>
</tr>
<tr>
<td>Lysogeny broth (LB)</td>
<td>10 g/L tryptone, 5 g/L yeast extract, 10 g/L NaCl, pH 7.0.</td>
</tr>
<tr>
<td>LB-agar plates (Amp)</td>
<td>20 g/L Bacto Agar in 500 mL dH<sub>2</sub>O, 100 µg/mL
Ampicillin.</td>
</tr>
</tbody>
</table>
</figure>

<figure id="tbl:ex3cells" class="align-left" style="width: 100%; float: left; margin-right: 1em">
  <figcaption style="font-size: 0.9em; color: #555; margin-bottom: 0.5em; line-height: 1.5; font-style: normal; display: block;">
    <strong style="color: #333;">Table 18.</strong> Cells
  </figcaption>
<table>
<thead>
<tr>
<th>Name</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td>HeLa</td>
<td><em>H. sapiens</em> cervix carcinoma derivative, epithelial-like,
(ACC 57, DSMZ).</td>
</tr>
<tr>
<td><em>E. coli</em> TOP10</td>
<td>Chemically-competent cells. Genotyp: F-<em>mcrA</em>
Δ(<em>mrr-hsd_RMS-</em>mcr_BC) Φ80<em>Lac</em>ZΔM15 Δ<em>Lac</em>X74
<em>rec</em>A1 <em>ara</em>D139 Δ(<em>araleu</em>) 7697 <em>gal</em>U
<em>gal</em>K <em>rps</em>L (StrR) <em>end</em>A1 <em>nup</em>G.</td>
</tr>
</tbody>
</table>
</figure>

<figure id="tbl:exp3buffers" class="align-left" style="width: 100%; float: left; margin-right: 1em">
  <figcaption style="font-size: 0.9em; color: #555; margin-bottom: 0.5em; line-height: 1.5; font-style: normal; display: block;">
    <strong style="color: #333;">Table 19.</strong> Buffers and chemicals
  </figcaption>
<table>
<thead>
<tr>
<th>Name</th>
<th>Description/Concentration</th>
</tr>
</thead>
<tbody>
<tr>
<td>PBS</td>
<td>2.7 mM KCl, 1.5 mM KH<sub>2</sub>PO4, 8.0 mM Na<sub>2</sub>HPO4, 137
mM NaCl in dH<sub>2</sub>O</td>
</tr>
<tr>
<td>Trypsin/EDTA in PBS</td>
<td>0.05% Trypsin/ 0.02% EDTA in PBS; PAN Biotech Cat.
No. P10-023500</td>
</tr>
<tr>
<td>RES/P1</td>
<td>50 mM Tris-HCl, 10 mM EDTA, 100 μg/mL RNase A, dH<sub>2</sub>O to 1
L</td>
</tr>
<tr>
<td>LYS/P2</td>
<td>0.2 M NaOH, 1% SDS, dH<sub>2</sub>O to 1 L</td>
</tr>
<tr>
<td>NEU/P3</td>
<td>3.0 M potassium acetate, dH<sub>2</sub>O to 1 L</td>
</tr>
<tr>
<td>EQU</td>
<td>750 mM NaCl, 50 mM MOPS, 15% isopropanol, 0,15% Triton X-100,
dH<sub>2</sub>O to 1 L</td>
</tr>
<tr>
<td>WASH</td>
<td>1.0M NaCl, 50 mM MOPS, 15% isopropanol, dH<sub>2</sub>O to 1 L</td>
</tr>
<tr>
<td>ELU</td>
<td>1.25M NaCl, 50 mM Tris-Cl, 15% isopropanol, dH<sub>2</sub>O to 1
L</td>
</tr>
<tr>
<td>2-Propanol</td>
<td>(Sigma)</td>
</tr>
<tr>
<td>70% Ethanol</td>
<td>70 ml Ethanol absolute (Chemsolute), dH<sub>2</sub>O to 100 mL</td>
</tr>
<tr>
<td>H<sub>2</sub>O</td>
<td></td>
</tr>
<tr>
<td>Polyethyleneimine (PEI)</td>
<td>1 mg/mL PEI (25 kDa) in dH<sub>2</sub>O, pH 7 (HCl), sterile
filtered with 0.2 μM pore size</td>
</tr>
<tr>
<td>Mowiol (Roth)</td>
<td>6 g glycerol, 2.4 g Mowiol 4-88, 6 mL dH<sub>2</sub>O, 12 mL 0.2 M
Tris-HCl pH 8.5</td>
</tr>
<tr>
<td>DABCO (Roth)</td>
<td>1,4-diazabicyclo[2.2.2]octane (anti-photobleaching reagent)</td>
</tr>
</tbody>
</table>
</figure>

<figure id="tbl:exp3cons" class="align-left" style="width: 100%; float: left; margin-right: 1em">
  <figcaption style="font-size: 0.9em; color: #555; margin-bottom: 0.5em; line-height: 1.5; font-style: normal; display: block;">
    <strong style="color: #333;">Table 20.</strong> Consumables
  </figcaption>
<table>
<thead>
<tr>
<th>Name</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td>Midi Columns</td>
<td>NucleoBond Xtra Midi Kit; Macherey-Nagel REF. 740410<br></td>
</tr>
<tr>
<td>24-well plates</td>
<td>Costar® 24-well Clear TC-treated Multiple Well Plates, cat.
No. 3524.</td>
</tr>
</tbody>
</table>
</figure>

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

1.  Harvest 100 mL culture by centrifugation twice for 5 min at 5,000 *xg* at RT in a 50 mL Falcon tube.
2.  Remove the supernatant (SN).
3.  Store the cell pellet at -20°C.

#### Day 10: Plasmid Midiprep

1.  Add 8 mL of buffer RES supplemented with RNAase (M. Nagel, 60 µg/mL) to the Falcon tube, thoroughly resuspend the cells.
2.  Add 8 mL lysis buffer LYS (if you notice precipitated SDS, warm it first until it dissolves). Mix by inverting 6 to 8 times. DO NOT VORTEX.
3.  Incubate 5 min at RT.
4.  Add 8 mL neutralization buffer NEU. Mix immediately by inverting the tube 6 to 8 times. DO NOT VORTEX.
5.  Centrifuge 10 min, 12,000 *xg* at RT. (Afterwards, pre-chill the centrifuge at 4°C for a later step. Do not forget to add the tube adapters.)
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
18. Air-dry the pellet (a few hours at RT, or in the oven at 65°C for approx. 5 min).
19. Resuspend with 70–120 µL ddH$`_2`$O (sterile).
20. Incubate 30 min at 37°C, resuspend by gentle pipetting.
21. Dilute the DNA 1:10 and determine the concentration using the nanodrop (eventually adjust the concentration to 2 µg/µL).
22. Store the extracted plasmids at -20°C.

#### Day 11: Seeding HeLa Cells on Glass Coverslips

This step should be performed only by one member of each group in order to prevent overcrowding in the cell culture room. Together with the supervisors, you will prepare a shared cell suspension. Each present group member will then seed the required number of cells in a 24-well plate (one plate per group)

1.  Prepare a 15 mL Falcon tube containing 8 mL prewarmed DMEMcomplete medium.
2.  Remove supernatant (pump).
3.  Gently add 2 mL prewarmed PBS, and tilt the plate to wash the cells. Remove the PBS again.
4.  Add 2 mL Trypsin and incubate the plate for 5 min at 37°C.
5.  Detach and resuspend the cells using a 1000 µL pipette. Transfer the suspension to the prepared medium. (The serum in the medium will inactivate the Trypsin).
6.  Centrifuge cells for 3 min, 300 *xg*.
7.  Remove supernatant and resuspend the cell pellet with 10 mL fresh medium.
8.  Prepare the Countess 3 counting chamber.
9.  Add 10 µL of the cell suspension to the cup.
10. Count cells using the Countess 3.
11. The Countess 3 provides information on the concentration (cells/mL) and viability (in %) of the cells. Please record this information for your protocol.
12. Determine the number of cells: counted cells/mL * 10 mL (volume) = total cells.
13. Seed HeLa cells as follows:

- Prepare a cell suspension with a concentration of 60,000 cells/mL (→ *c2)* by dilution with DMEMcomplete medium. Prepare 35 mL (→ *v2)* of cell suspension in order to have enough for all groups. Use a 50 mL Falcon tube. The required dilution volume *v1* can be calculated according to the formula *c1* * *v1* = *c2* * *v2*.
- Seed 500 µL of cell suspension (containing 30,000 HeLa cells) into each well of a 24-well plate **containing a glass cover slip** (prepared by supervisors in advance). Each group should seed 6 wells into an individual plate.

<figure id="tbl:yourtablelabel" class="align-center" style="width: 30%; display: block; margin-left: auto; margin-right: auto">
  <figcaption style="font-size: 0.9em; color: #555; margin-bottom: 0.5em; line-height: 1.5; font-style: normal; display: block;">
    <strong style="color: #333;">Table 21.</strong> Well plate layout: Seed wells 1, 2, and 3 in a 24-well plate (6 wells per group).
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

13. Place the cell culture plate into the 37°C incubator to allow them to attach to the glass coverslip for the PEI transfection on day 12.

#### Day 12: PEI Transfection

1.  Per well, dilute 0.75 µg of DNA in OptiMEM to a final volume of 50 µL (remember your Midi-prep concentration). Please check **[Table 22](#tbl:transfection-odd)** and **[Table 23](#tbl:transfection-even)** for further information.
2.  When transfecting multiple plasmids for the same setup, divide the total DNA amount (0.75 µg) by the number of plasmids which are transfected (equal plasmid load). Note: keep ca. 0.75 µg as total DNA amount; the ratio of DNA: PEI is important for the transfection efficiency!
3.  Per well, dilute 2.5 µL of PEI solution in OptiMEM to a final volume of 50 µL. Vortex. Please check **[Table 22](#tbl:transfection-odd)** and **[Table 23](#tbl:transfection-even)** for further information.
4.  Add an equal volume of PEI solution to the DNA solution.
5.  Vortex the solution immediately and thoroughly for 10 s. Complexation of PEI with DNA, into small particles able to enter the cell during transfection, is dependent on thorough mixing at this step.
6.  Incubate for 15 min at RT.
7.  Per well, add the premixed 100 µL PEI/DNA mix drop-wise to each well. DO NOT VORTEX!
8.  Incubate for 4 h at 37°C in the cell culture incubator.
9.  Exchange medium for fresh cultivation medium (500 µL per well).

<figure id="tbl:transfection-odd" class="align-left" style="width: 100%; float: left; margin-right: 1em">
  <figcaption style="font-size: 0.9em; color: #555; margin-bottom: 0.5em; line-height: 1.5; font-style: normal; display: block;">
    <strong style="color: #333;">Table 22.</strong> Transfection Set up 1 for odd group numbers.
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
  <figcaption style="font-size: 0.9em; color: #555; margin-bottom: 0.5em; line-height: 1.5; font-style: normal; display: block;">
    <strong style="color: #333;">Table 23.</strong> Transfection Set up 1 for even group numbers.
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
9.  Briefly dip the cover slip into water.
10. Carefully get rid of water droplets with the help of fine tissue.
11. Place the coverslips with the cells facing down onto the Mowiol droplet. Avoid air bubbles.
12. Dry slides at 37°C for 30 min.

#### Confocal Microscopy

One pair of odd and even group members proceeds to the confocal microscope at a time, accompanied by their supervisors. Afterwards, you may analyze the data using FIJI in the seminar room.

----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

[← Previous](garden_05-Experiment3.md) \| [Next →](garden_07-Experiment5.md)
