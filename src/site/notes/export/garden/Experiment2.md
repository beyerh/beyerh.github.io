---
{"dg-publish":true,"permalink":"/export/garden/experiment2/"}
---

## Experiment II: Optogenetic Gene Expression Using Stably-Engineered Mammalian Cells

**Supervisors**: Benjamin McLean, Daniel Wiebensohn, Miriam Labusch

The objective of this experiment is to learn how to control and analyze the induction of gene expression via an optogenetic tool in mammalian cells. To this end, foreign genes encoding the photo-switch and a light-inducible reporter encoding a gene of interest were previously introduced into the genome of Chinese Hamster Ovary (CHO-K1) cells. We will treat this customized cell line with light and dark and quantify the reporter expression over a time course of 24 hours.

Transient transfection is an efficient method for preliminary reporter assays. CHO-K1 cells normally achieve high transfection rates and express recombinant proteins in large scale when using polyethylenimine (PEI)-based transient transfection methods (see introduction **Figure split-intein-apps**). In contrast to many commercial transfection agents, PEI is inexpensive yet very efficient for a range of mammalian cell lines. However, the transfection efficiency can be affected by various parameters (cell type, number of plasmids, DNA amount, DNA quality, etc.). Additionally, in transiently transfected cells, the foreign DNA rarely integrates into the host genome and consequently does not replicate, leading to an eventual loss through cycles of cell division over several days.

Stable genomic integration is often the preferred option as the foreign gene becomes part of the genome which allows for greater process consistency and long-term protein expression. However, the generation of stable cell lines is a time-consuming and expensive process. In this experiment, we will provide a stably-engineered CHO-K1 cell line generated using a sequential genomic integration of two vectors (**Figure 1**). One vector encodes an optogenetic LOVpep/ePDZ-based split transcription factor system under the selection of puromycin, and the other a SEAP reporter under the selection of Hygromycin. The principle of generating stable cell lines using the Sleeping Beauty transposase is explained in the introduction part (**Figure sleeping-beauty**).

The following experiment will be about handling mammalian cell culture as well as the analysis of a light-induced reporter gene. The human placental **se**creted **a**lkaline **p**hosphatase (SEAP) as a reporter has tremendous advantages. SEAP is very stable, and its secretion into the medium allows a convenient and non-invasive way of acquiring samples. Furthermore, it is a quantitative reporter for gene expression because the SEAP activity in the supernatant of transfected CHO-K1 cells is proportional to shifts in intracellular SEAP mRNA levels. The activity of promoters/enhancers and other elements can be measured due to their direct correlation to SEAP secretion. Finally, the SEAP phosphatase is heat persistent and endures a temperature of 65°C, whereas other phosphatases degrade at this temperature. Therefore, heat treatment can be used to selectively enrich SEAP in samples that might contain additional phosphatases.

<figure id="fig:optogenetic-switch" class="align-left" style="width: 100%; display: block; margin-right: auto">

![Figure 1](/img/user/figures/BLUE_gene_switch.png)

<figcaption>
<strong>Figure 1.</strong> 
<strong>Mode of function of the optogenetic gene switch in
genomically-engineered cells.</strong> <strong>A)</strong> An engineered
LOV2 domain from <em>Avena sativa</em> phototropin 1 was fused to the
C-terminus of the E-protein (erythromycin resistance protein), thus
tethering it to a response construct harboring 8 repeats of the E
binding sequence (<em>etr8</em>) upstream of a synthetic minimal
promoter, while the PDZ interaction domain was fused to the VP16
transactivation domain. In the dark, the epitope tag of the LOVpep
fusion protein is inaccessible for the PDZ domain. Consequently, gene
expression is off. Blue light (460 nm) illumination leads to the
unwinding of the C-terminal Jα helix of LOVpep and makes the epitope tag
accessible for binding of the PDZ domain. Due to the recruitment of the
transactivator VP16 to the minimal promoter, the transcriptional
machineries are recruited, and the SEAP gene‑expression is induced.
Schematic representation of the vector encoding the photo-switch
<strong>(B)</strong> and the SEAP reporter gene <strong>(C)</strong>
both flanked by inverted terminal repeats (ITRs).
</figcaption>
</figure>

### Materials

<figure id="tbl:materials-exp2" class="align-left" style="width: 100%; float: left; margin-right: 1em">
  <figcaption>
    <strong>Table 1.</strong> 

  </figcaption>
<table>
<thead>
<tr>
<th>Item</th>
<th>Composition/Concentration</th>
<th>Application</th>
</tr>
</thead>
<tbody>
<tr>
<td>Ham’s Medium</td>
<td>90% Ham’s tissue culture medium F12 (PAN-Biotech), 10% fetal bovine
serum (FBS, PAN-Biotech), 100 U/mL penicillin, 0.1 mg/mL streptomycin
(Gibco).</td>
<td>Growth medium</td>
</tr>
<tr>
<td>Trypsin/EDTA in PBS</td>
<td>0.05% Trypsin/ 0.02% EDTA in PBS; (PAN Biotech Cat.
No. P10-023500)</td>
<td>Cell dissociation</td>
</tr>
<tr>
<td>1x PBS</td>
<td>2.7 mM KCl, 1.5 mM KH<sub>2</sub>PO<sub>4</sub>, 8.0 mM
Na<sub>2</sub>HPO<sub>4</sub>, 137 mM NaCl in dH<sub>2</sub>O.</td>
<td>Removal of dead cells</td>
</tr>
<tr>
<td>2x SEAP buffer</td>
<td>20 mM homoarginine, 1 mM MgCl<sub>2</sub>, 21% (v/v) diethanolamine,
pH 9.8</td>
<td>Inhibition of endogenous phosphatases</td>
</tr>
<tr>
<td>pNPP</td>
<td>120 mM in dH<sub>2</sub>O</td>
<td>SEAP substrate</td>
</tr>
</tbody>
</table>
</figure>

### Protocol

#### Day 3: Seeding Mammalian Cells 

Preparation of materials:

-   Pre-warm Ham’s medium, 1X PBS, and Trypsin/EDTA in 37°C water bath.
-   15 mL falcons, stripette tips (10 mL), 1000 µL and 200 µL tips (sterilized).
-   24-well cell-culture plates for cell seeding.
-   Fuchs-Rosenthal counting chamber.

Procedure:

1.  Perform all steps under **green safelight** to avoid exposure to ambient light.
2.  Check cell confluency briefly under the microscope.
3.  Introduce medium, PBS, and Trypsin into the laminar flow bench and screw all lids open  
    (do not remove the lids).
4.  Remove supernatant (with yellow tip using the pump).  
    Tilt the petri dish toward you gently, remove the supernatant, and avoid touching the cells.
5.  Add 2 mL PBS to wash, then remove it.
6.  Add 2 mL Trypsin and ensure that all cells are covered. Incubate for 5 min at 37 °C in the incubator.
7.  Meanwhile, prepare a 15 mL Falcon tube with 8 mL of medium.
8.  Fully detach and resuspend the cells in the Trypsin solution after the 5 min incubation. Transfer the Trypsin/cell suspension to the Falcon tube with the prepared medium and gently invert.
9.  Centrifuge cells for 3 min at 300 g. Meanwhile, prepare the Fuchs-Rosenthal chamber for cell counting.
10. Remove the supernatant with the pump or by decanting.
11. Add 10 mL of fresh medium and resuspend.
12. Count cells using the Fuchs-Rosenthal counting chamber.

**① Calculate Original Cell Concentration ($C_{\text{orig}}$)**

First, determine the concentration of your stock solution in $\text{cells/mL}$. For a Fuchs-Rosenthal chamber ($0.2\text{ mm}$ depth, $1\text{ mm}^2$ large square area), the volume of one large square is $0.2\ \mu\text{L}$ (which is $1/5,000$ of a mL).

$$C_{\text{orig}}\ (\text{cells/mL}) = \frac{\text{Total Cells Counted}}{\text{Number of Squares Counted}} \times 5,000 \times \text{Dilution Factor}$$

**② Define Target Seeding Concentration ($C_{\text{target}}$)**

Next, calculate the concentration of the working solution you need for your plates.

$$C_{\text{target}}\ (\text{cells/mL}) = \frac{\text{Target Cells per Well}}{\text{Volume per Well (mL)}}$$

> *Example: If seeding $50,000\text{ cells}$ in $500\ \mu\text{L}$ ($0.5\text{ mL}$) per well, your target concentration is $50,000 \div 0.5 = 100,000\text{ cells/mL}$.*

**③ Calculate Total Master Mix Volume ($V_{\text{total}}$)**

To avoid running out of suspension due to pipetting inaccuracies, always calculate for your planned wells plus a safety margin ($W_{\text{extra}}$, typically 10% extra or 1-2 extra wells).

$$W_{\text{total}} = W_{\text{planned}} + W_{\text{extra}}$$

$$V_{\text{total}}\ (\text{mL}) = W_{\text{total}} \times \text{Volume per Well (mL)}$$

**④ Calculate Mixing Volumes ($V_{\text{suspension}}$ and $V_{\text{medium}}$)**

Finally, use the $C_1V_1 = C_2V_2$ formula to determine how much original cell suspension to mix with fresh medium to create your master mix.

**Determine volume of original cell suspension needed:**

$$V_{\text{suspension}}\ (\text{mL}) = \frac{C_{\text{target}} \times V_{\text{total}}}{C_{\text{orig}}}$$

**Determine volume of fresh medium needed to reach final volume:**

$$V_{\text{medium}}\ (\text{mL}) = V_{\text{total}} - V_{\text{suspension}}$$

**Next Step at the Bench:** Add $V_{\text{suspension}}$ of your cells to a sterile tube containing $V_{\text{medium}}$ of fresh medium. Mix gently, then pipette your standard volume (e.g., $500\ \mu\text{L}$) into each well.

1.  For each group: 4 wells as replicates of each time point (t1 and t2), 2 different incubation conditions (light and dark), therefore prepare 16+1 wells per group and seed into 2 **different** plates!
2.  Prepare the calculated cells suspension (50,000 cells per well) and medium in a 50 mL falcon (master mix).
3.  Add 500 µL to each well.

Incubate the cells overnight at 37°C in the CO~2~ incubator.

#### Day 4: Illumination / t0 and t1 Supernatant Collection 

Preparation of materials:

-   Pre-warm Ham’s in a 37°C water bath.
-   15 mL Falcon tubes, stripette tips (10 mL), 1000 µL, and 200 µL tips.
-   Light boxes adjusted to blue light 460 nm with a light intensity of 10 μmol m^-2^ s^-1^.
-   Round bottom 96-well plate.

Procedure:

1.  Check the cells under the microscope.

For collecting the t0 sample, we will proceed as follows:

-   Groups 1-4 will take the supernatant without any medium change.
-   Groups 5-8 will perform a medium change before taking the supernatant.

1.  Take 200 µL supernatant from each well into the 96-well plate as “0 h” sample (Groups 1-4).
2.  Remove the rest medium and add 500 µL of fresh medium into each well.
3.  Transfer 200 µL of the freshly exchanged medium from each well into the 96-well plate as “0 h” sample (Groups 5-8). Replace the 200 µL taken.
4.  Transfer one of your 24-well plates into a light box with 10 μmol m^-2^ s^-1^ blue light and the other one into the dark box.
5.  After 6 h illumination, take 200 µL supernatant from the t1 wells of each plate into the 96-well plate (clear, round bottom) in the laminar flow bench under green light. Return the cells to the light boxes in the incubator.
6.  Seal the 96-well plate with tape (make sure it is well sealed).
7.  Store at -20°C.

#### Day 5: t2 Supernatant Collection and SEAP Assay 

Preparation of materials:

-   Transparent 96-well plate (flat bottom).
-   2x SEAP buffer and para-nitrophenyl-phosphate (pNPP) substrate.
-   PBS.
-   Multichannel and multi-stepper pipettes with tips.

1.  After 24 h illumination, transfer 200 µL of cell supernatant from the t2 wells into the 96-well plate.
2.  Incubate the sealed round-bottom 96-well plate for 45 min at 65°C.
3.  Add 100 µL of SEAP buffer into each well of a flat-bottom 96-well plate using the multi-stepper pipette.
4.  Add 80 µL of supernatant from the round-bottom 96-well plate. For samples from timepoint t2, first add 40 µL PBS and then only 40 µL of supernatant.
5.  Set up the program at the plate reader (Absorbance 1h: spectroscopic measurement every minute (60 times, ca. 1 h); wavelength 405 nm.)
6.  Remove air-bubbles with toothpicks.
7.  Add 20 µL of pNPP substrate using the multi-stepper pipette. Be fast, as the reaction starts immediately after adding the substrate to the first well. One person should add the substrate for the entire plate. Place the plate immediately into the plate reader and start the measurement.

<figure id="fig:seap-formula" class="align-left" style="width: 80%; display: block; margin-right: auto">

![Figure 2](/img/user/figures/seap_formula.png)

<figcaption>
<strong>Figure 2.</strong> 
Pipetting scheme.
</figcaption>
</figure>

Hints for data processing:

Subsequent determination of the SEAP activity \[U/L\] is performed by calculating the slope of the  
respective curves \[OD/min\] and the Lambert-Beer law, resulting in the following formula:

∈ = 18,600 M^-1^cm^-1^; d= length of the light path \[cm\] (typically 0.5 cm); = amount of SEAP‑containing supernatant / dilution factor of the sample; = used volume of supernatant.

It is highly recommended to develop a template with Microsoft Excel for data processing.

----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

\[\[Experiment1\|← Previous\]\] \| \[\[Experiment3\|Next →\]\]
