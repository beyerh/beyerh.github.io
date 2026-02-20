---
{"dg-publish":true,"permalink":"/export/garden/06-experiment5/"}
---

## Experiment V: Engineering Chemically Regulated Gene Switch Technology in Stable Mammalian Cell Culture

**Supervisors:** Maria Evangelopoulou, Miriam Labusch, Benjamin McLean

### Aim

The aim of this experiment is to investigate the dose-dependent induction of neonGreen expression using the tetracycline-inducible system and quantify fluorescence levels via flow cytometry. Each group will generate stable transgenic CHO-K1 lines carrying both the reporter and tetR, and will then measure fluorescence in a control sample without tetracycline, as well as in one experimental sample containing a given tetracycline concentration to compare expression levels.

### Background

#### Tetracycline-Inducible Expression System (Tet System)

The tetracycline (Tet) system is a widely used inducible gene expression system that enables precise control over the transcription of a gene of interest. It is based on regulatory elements derived from the *Escherichia coli* tetracycline resistance operon. The system typically consists of two components:

1.  A **t**etracycline-controlled **t**rans**a**ctivator (tTA or rtTA-reverse rTA), which binds to tetracycline response elements (TRE) upstream of the gene of interest.
2.  The target gene, in this case coding for the fluorescent protein neonGreen, downstream of the TRE.

<figure id="fig:tet-system" class="align-left" style="width: 60%; display: block; margin-right: auto">

![Figure 1](/img/user/figures/Tet-On.png)

<figcaption>
<strong>Figure 1.</strong> 
** Schematic representation of the Tet-On system.** The Tet-On 3G
protein is constitutively expressed under the control of the CAG
promoter. Upon addition of tetracycline, the Tet-On 3G protein undergoes
a conformational change that enables it to bind to the TRE3G promoter,
thereby activating transcription and inducing neonGreen expression.
</figcaption>
</figure>

In our experiment, we will implement the Tet-On system in a 3G (third-generation) configuration, which uses an optimized reverse tetracycline-controlled transactivator to achieve tighter regulation and higher sensitivity to induction. In the Tet-On system, gene expression is activated in the presence of tetracycline or its derivative doxycycline. When tetracycline is added to the cells, it binds to the Tet (rtTA/tTA) protein and alters its conformation, enabling it to interact with the TRE promoter and thereby activate gene transcription (in our case: NeonGreen). The amount of tetracycline added determines the extent of activation, allowing for dose-dependent regulation of expression.

#### Why Different Concentrations Matter

Using different tetracycline concentrations enables fine-tuning of expression levels. At low concentrations, only a small fraction of rtTA will be activated, resulting in weak expression. Higher concentrations lead to stronger induction and higher levels of fluorescent protein. However, once all Tet proteins are bound by tetracycline, the system reaches saturation, and further increases in concentration will no longer enhance expression levels. Excessively high concentrations may further cause off-target effects and cellular stress leading to non-linear responses. This dose-dependent approach therefore helps to:

- Establish induction thresholds
- Analyze the dynamic range of the system
- Investigate potential cytotoxicity or system leakage
- Determine optimal working concentrations for controlled expression

#### Flow Cytometry for Quantifying Fluorescent Reporters

**Analyzing the induction with the flow cytometer**

To measure neonGreen expression on a single-cell level, a flow cytometer is used. Flow cytometry allows rapid analysis of thousands of individual cells as they pass through a laser beam in a fluid stream. When the laser excites the fluorescent reporter (neonGreen), the emitted light is detected by photomultiplier tubes and converted into numerical fluorescence intensity values. This enables quantitative measurement of expression levels within cell populations.

**Advantages of Flow Cytometry**

- Single-cell resolution allows detection of heterogeneous expression patterns.
- High throughput: thousands of cells per second can be analyzed.
- Quantitative: provides precise fluorescence intensity values.
- Multi-parameter analysis: expression can be correlated with other markers (e.g., viability or cell cycle).

#### Stable Cell Lines and Their Advantages

Stable cell lines are cell populations that have stably integrated foreign DNA into their genome, allowing long-term and consistent expression of the gene of interest. Unlike transient transfections, where the introduced DNA is only temporarily present and expression levels vary between cells and over time, stable lines provide reproducible and uniform expression profiles across experiments. Testing the tet-inducible system in stable lines offers several advantages: it ensures reliable control of gene expression, reduces variability between samples, and allows for more accurate quantification of induction levels. Additionally, stable integration enables long-term experiments and repeated induction studies without the need to transfect cells again, making it ideal for analyzing dose-dependent responses and optimizing tetracycline concentrations.

### Material

<figure id="tbl:materials-exp5" class="align-left" style="width: align; float: left; margin-right: 1em">
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
<td>Trypsin</td>
<td>0.05% Trypsin</td>
<td>Cell dissociation</td>
</tr>
<tr>
<td>1x PBS</td>
<td>2.7 mM KCl, 1.5 mM KH<span
class="math inline"><sub>2</sub></span>PO<span
class="math inline"><sub>4</sub></span>, 8.0 mM Na<span
class="math inline"><sub>2</sub></span>HPO<span
class="math inline"><sub>4</sub></span>, 137 mM NaCl in dH<span
class="math inline"><sub>2</sub></span>O.</td>
<td>Removal of dead cells &amp; Dilution of cells for measurement</td>
</tr>
<tr>
<td>Puromycin</td>
<td>10 mg/mL Puromycin</td>
<td>Antibiotic for selection</td>
</tr>
<tr>
<td>Tetracycline</td>
<td>1000 µg/mL Tetracycline</td>
<td>Induction of neonGreen expression</td>
</tr>
<tr>
<td>Polyethylenimine (PEI)</td>
<td>1 mg/mL polyethylenimine</td>
<td>Transfection reagent</td>
</tr>
<tr>
<td>OptiMEM</td>
<td>OptiMEM reduced serum medium (Gibco).</td>
<td>Transfection medium</td>
</tr>
</tbody>
</table>
</figure>
<figure id="tbl:exp5plasmids" class="align-left" style="width: 100%; float: left; margin-right: 1em">
  <figcaption>
    <strong>Table 2.</strong> 
Used plasmids prepared by the supervisors.
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
<td>pDD312</td>
<td>PCAG-TetOn3G-Tbg - Ptre3gv-mneonGreen-TSV40</td>
<td>1926 ng/µL</td>
</tr>
<tr>
<td>pME001</td>
<td>PT7-PB transposase- TSV40</td>
<td>2126 ng/µL</td>
</tr>
</tbody>
</table>
</figure>

### Protocol

#### Day 2 - Cell Seeding (will be performed by your supervisors)

**What you will need**

- Pre-warmed HAMs medium, 1x PBS, and Trypsin (37°C water bath)
- 15 mL falcons, 10 mL stripette tips, 200 µL and 1000 µL sterile tips
- 6-well culture plate for cell seeding
- Fuchs-Rosenthal counting chamber

**Procedure**

1.  Prepare the clean bench: clean with ethanol, then introduce medium, PBS and trypsin, falcons and tips by vigorously spraying them down with ethanol.
2.  Check cell confluency under microscope (ideally around 70 - 90%) before introducing the plate into the clean bench.
3.  Remove supernatant using the pump with a yellow tip → tilt the petri dish toward you and remove supernatant without touching the cells.
4.  Add 2 mL PBS to wash the cells and remove it.
5.  Add 2 mL trypsin and ensure all cells are covered → incubate for 5 min at 37°C in the incubator.
6.  Meanwhile, prepare a 15 mL falcon tube with 5 mL HAMs medium.
7.  After the 5 min incubation, make sure to fully detach cells by resuspending the trypsin solution and transfer everything into the freshly prepared falcon with medium.
8.  Centrifuge cells for 3 min at 300 g.
9.  Meanwhile, prepare the Fuchs-Rosenthal chamber in order to count the cells.
10. Remove the supernatant from the cells using the pump.
11. Resuspend the cells in 10 mL of fresh HAMs medium.
12. Count cells with Fuchs-Rosenthal counting chamber using \~ 15 µL → you need to count at least 4 squares and calculate the amount for the whole chamber (16 squares, depth = 0.2 mm, A = 0.0625 mm$^2$, 1 mm$^3$ = 1 µL).

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

#### Day 3 - Stable Transfection

For this part of the experiment three groups will form one big group to transfect one well per group, so in the end we would have three transfected wells. These groups will then share the responsibility of passaging and selecting the cells until the day of seeding for the experiment.

**What you will need**

- Pre-warmed OptiMEM (37°C water bath)
- Polyethyleneimine (PEI)
- 1.5 mL tubes, 10 µL, 200 µL and 1000 µL sterile tips
- Cells seeded in 6-well plate
- Plasmids: pME001 (piggybac transposase), pDD312 (tet inducible neonGreen expression)

<figure id="tbl:yourtablelabel" class="align-left" style="width: 100%; float: left; margin-right: 1em">
  <figcaption>
    <strong>Table 3.</strong> 
<strong>Here we still need to add a table as pdf figure</strong>
  </figcaption>
<table>
<thead>
<tr>
<th>Column A</th>
<th>Column B</th>
<th>Column C</th>
</tr>
</thead>
<tbody>
<tr>
<td></td>
<td></td>
<td></td>
</tr>
</tbody>
</table>
</figure>

**Procedure**

1.  Calculate the volumes needed for OptiMEM and the respective plasmids.
2.  Prepare OptiMEM-DNA mix based on your calculations and vortex.
3.  Prepare PEI/OptiMEM Mix.
4.  Add PEI/OptiMEM to your DNA mix and vortex for 10 s.
5.  Incubate for 20 min at room temperature.
6.  Add 500 µL dropwise to each well and distribute by moving plate from side to side.
7.  Medium exchange \~ 4 h after transfection.
8.  Aspirate medium and add 2 mL fresh DMEM.

#### Day 5 – Split Cells and Start Selection

Two days after transfection, the selection process is initiated using the antibiotic encoded in the selection cassette of the transfected plasmid pDD312. In this case, the antibiotic is puromycin. In addition to the antibiotic resistance gene, the selection cassette also encodes a blue fluorescent protein (BFP), which serves as an additional selection marker. During the selection period, the efficiency and progression of selection can be monitored by visualizing BFP expression under a fluorescence microscope.

**What you will need**

- Pre-warmed HAMs medium, 1x PBS, and Trypsin (37°C water bath)
- 15 mL falcons, 10 mL stripette tips, 200 µL and 1000 µL sterile tips
- 10 cm petri dish
- Puromycin (10 µg/mL)

**Procedure**

1.  Prepare the clean bench: clean with ethanol, then introduce medium, PBS and trypsin, falcons and tips by vigorously spraying them down with ethanol.
2.  Check cell confluency under microscope (ideally around 70 - 90%) and fluorescence of your BFP fluorescence reporter, before introducing the plate into the clean bench.
3.  Remove supernatant using the pump with a yellow tip → tilt the plate toward you and remove supernatant without touching the cells.
4.  Add 1 mL PBS to wash the cells and remove it.
5.  Add 1 mL trypsin and ensure all cells are covered → incubate for 5 min at 37°C in the incubator.
6.  Meanwhile, prepare a 15 mL falcon tube with 3 mL HAMs medium.
7.  After the 5 min incubation, make sure to fully detach cells by resuspending the trypsin solution and transfer everything into the freshly prepared falcon with medium.
8.  Centrifuge cells for 3 min at 300 g.
9.  Meanwhile prepare a 10 cm petri dish with 10 mL HAMs medium.
10. Remove supernatant and add 1 mL of fresh medium.
11. Transfer the cell suspension onto your petri dish.
12. Add 10 µL of puromycin (10 µg/mL) and distribute cells and antibiotic by moving the plate (e.g., gently rocking).

#### Day 6 - Change Medium or Split Culture

Depending on the transfection efficiency the transfected cells could we ready to split again. If not, we will just perform a medium change and add new puromycin for selection.

**What you will need**

- Pre-warmed HAMs medium, 1x PBS, and Trypsin (37°C water bath)
- 15 mL falcons, 10 mL stripette tips, 200 µL and 1000 µL sterile tips
- 10 cm petri dish
- Puromycin (10 µg/mL)

**Procedure**

1.  Prepare the clean bench: clean with ethanol, then introduce medium, PBS and trypsin, falcons and tips by vigorously spraying them down with ethanol.
2.  Check cell confluency under microscope (ideally around 70 - 90%) and fluorescence of your BFP fluorescence reporter, before introducing the plate into the clean bench.
3.  Remove supernatant using the pump with a yellow tip → tilt the plate toward you and remove supernatant without touching the cells.
4.  Add 2 mL PBS to wash the cells and remove it.
5.  Add 2 mL trypsin and ensure all cells are covered → incubate for 5 min at 37°C in the incubator.
6.  Meanwhile, prepare a 15 mL falcon tube with 5 mL HAMs medium.
7.  After the 5 min incubation, make sure to fully detach cells by resuspending the trypsin solution and transfer everything into the freshly prepared falcon with medium.
8.  Centrifuge cells for 3 min at 300 g.
9.  Meanwhile prepare a 10 cm petri dish with 10 mL HAMs medium.
10. Remove supernatant and add 2 mL of fresh medium.
11. For ratio splitting: in a 1:16 ratio add 125 µL of cell suspension to your new culture dish.
12. Add 10 µL of puromycin (10 µg/mL) and distribute cells and antibiotic by moving the plate.

#### Day 10 - Split Cells

**What you will need**

- Pre-warmed HAMs medium, 1x PBS, and Trypsin (37°C water bath)
- 15 mL falcons, 10 mL stripette tips, 200 µL and 1000 µL sterile tips
- 10 cm petri dish
- Puromycin (10 µg/mL)

**Procedure**

1.  Prepare the clean bench: clean with ethanol, then introduce medium, PBS and trypsin, falcons and tips by vigorously spraying them down with ethanol.
2.  Check cell confluency under microscope (ideally around 70 - 90%) and fluorescence of your BFP fluorescence reporter, before introducing the plate into the clean bench. → here we have to check if it is necessary to continue our selection.
3.  Remove supernatant using the pump with a yellow tip → tilt the plate toward you and remove supernatant without touching the cells.
4.  Add 2 mL PBS to wash the cells and remove it.
5.  Add 2 mL trypsin and ensure all cells are covered → incubate for 5 min at 37°C in the incubator.
6.  Meanwhile, prepare a 15 mL falcon tube with 5 mL HAMs medium.
7.  After the 5 min incubation, make sure to fully detach cells by resuspending the trypsin solution and transfer everything into the freshly prepared falcon with medium.
8.  Centrifuge cells for 3 min at 300 g.
9.  Meanwhile prepare a 10 cm petri dish with 10 mL HAMs medium.
10. Remove supernatant and add 2 mL of fresh medium.
11. For ratio splitting: in a 1:8 ratio add 250 µL of cell suspension to your new culture dish.
12. Add 10 µL of puromycin (10 µg/mL) and distribute cells and antibiotic by moving the plate. (If cell selection is complete, it may not be necessary to add puromycin today).

#### Day 11 - Cell Seeding for Experiment

In this part of the experiment, you are going to seed the generated stable cell culture into 6-well plates for the tetracycline induction. There you will be testing two conditions: one specific tetracycline concentration per group, and a negative control group (no tetracycline). This will be performed in technical triplicate for each condition. This means each group will be seeding one whole 6-well plate.

**What you will need**

- Pre-warmed HAMs medium, 1x PBS, and Trypsin (37°C water bath)
- 15 mL falcons, 10 mL stripette tips, 200 µL and 1000 µL sterile tips
- 6-well plates

**Procedure**

1.  Prepare the clean bench: clean with ethanol, then introduce medium, PBS and trypsin, falcons and tips by vigorously spraying them down with ethanol.
2.  Remove supernatant using the pump with a yellow tip → tilt the plate toward you and remove supernatant without touching the cells.
3.  Add 2 mL PBS to wash the cells and remove it.
4.  Add 2 mL trypsin and ensure all cells are covered → incubate for 5 min at 37°C in the incubator.
5.  Meanwhile, prepare a 15 mL falcon tube with 5 mL HAMs medium.
6.  After the 5 min incubation, make sure to fully detach cells by resuspending the trypsin solution and transfer everything into the freshly prepared falcon with medium.
7.  Centrifuge cells for 3 min at 300 g.
8.  Meanwhile prepare the chamber for cell counting using the Countess.
9.  Remove supernatant and add 10 mL of fresh medium.
10. Measure the cell concentration with the supervisors using the cell countess.
11. Based on your cell concentration calculate how many cells you will need to seed for your experiment. You will need 250,000 cells per well.
12. The supervisors will prepare a plate of wildtype CHO cells.

#### Day 12 - Tetracycline Induction

Here we are going to induce the expression of neonGreen using different concentrations of tetracycline. The group will be split in half: 4 groups will perform this experiment in the morning and the rest in the afternoon. The concentrations tested in the morning will be the same as in the afternoon. Note for the analysis part: show and discuss the results of the different concentrations in your protocol. The groups within the same timeslot will have to share their data with each other.

**What you will need**

- Pre-warmed HAMs medium
- 10 µL, 200 µL, and 1000 µL sterile tips
- Tetracycline (undiluted stock solution)

**Procedure**

1.  Prepare the clean bench: clean with ethanol, then introduce medium, PBS and trypsin, falcons and tips by vigorously spraying them down with ethanol.
2.  Remove supernatant using the pump with a yellow tip.
3.  Add 2 mL fresh medium to each well.
4.  Using 10 µL pipette tips, add the appropriate amount of tetracycline to each well. In each 6 well plate, 3 wells will remain without tetracycline (negative control). The remaining 3 wells will receive the same amount of tetracycline each (depending on your group). The following concentrations will be tested: X, X, X, and X).

#### Day 13 - Flow Cytometry

**What you will need**

- Pre-warmed HAMs medium, 1x PBS, and Trypsin (37°C water bath)
- 200 µL and 1000 µL sterile tips
- 1.5 mL Eppi tubes

**Preparations before the measurement**

1.  Prepare the clean bench: clean with ethanol, then introduce medium, PBS and trypsin, falcons and tips by vigorously spraying them down with ethanol.
2.  Remove supernatant using the pump with a yellow tip → tilt the petri dish toward you and remove supernatant without touching the cells.
3.  Add 200 µL PBS to wash the cells and remove it.
4.  Add 200 µL trypsin and ensure all cells are covered → incubate for 5 min at 37°C in the incubator.
5.  In the meantime: prepare + label 6 1.5 mL tubes for your measurement (labeling on the side of each tube!).
6.  Release all the cells from the culture dish by pipetting/ washing and stop the trypsin reaction with 600 µL medium.
7.  Transfer cell suspensions in designated 1.5 mL tubes.
8.  Centrifuge cells for 3 min at 300 g.
9.  Aspirate supernatant.
10. Resuspend w/ 100 µL PBS.
11. Cytometer Measurement

----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

\[\[05-Experiment4\|← Previous\]\] \| \[\[07-References\|Next →\]\]
