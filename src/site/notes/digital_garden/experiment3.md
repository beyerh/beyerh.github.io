---
{"dg-publish":true,"permalink":"/digital-garden/experiment3/"}
---



# Experiment III: Protein Trans-Splicing for Bacterial Logic Gate Design

**Supervisors:** Josepha Grewer, Maria Evangelopoulou, Hannes Beyer

josepha.grewer@hhu.de, cur91fom@hhu.de, hannes.beyer@hhu.de

In this experiment, we adapt the naturally occurring protein *cis*- and *trans*-splicing catalyzed by the DnaE intein from *Nostoc punctiforme* (*Npu*DnaE intein) to engineer a synthetic protein logic gate. As previously explained in section 1.1.2, inteins are protein domains with autocatalytic activity that give rise to a reconstituted functional protein after self-excising from the host or precursor protein. Protein splicing can occur either in *cis* (excision of an intein) or in *trans*, leading to the ligation of two individual proteins, each fused to one fragment of a split intein. In Experiment I, we have cloned the bacterial inducible plasmids that we need for this experiment (**Figure 13**):

- pDD259: IPTG-inducible promoter guiding the expression of mCherry fluorescent protein hosting a *cis*-splicing intein.
- pDD262: IPTG-inducible promoter guiding the expression of mCherry fluorescent protein hosting a *cis*-splicing intein with an inactivating mutation of Cys1 to Ala.
- pD260: IPTG-inducible promoter guiding the expression of the N-terminal region of mCherry fused to the N-terminal fragment of the *Npu*DnaE intein (Int~N~, N-terminal split fragment).
- pD261: Arabinose-inducible promoter guiding the expression of the C-terminal region of mCherry fused to the C-terminal fragment of the *Npu*DnaE intein (Int~C~, C-terminal split fragment).

We will transform and induce protein production in the *Escherichia coli* strain T7-Express using competent cells following the scheme in **Figure 13**:

- Transformation of pDD259: We will use this construct to test intein-based protein *cis*-splicing. Therefore, if the system is working properly, we should be able to detect mCherry fluorescence upon IPTG induction.
- Transformation of pDD262: The construct is almost identical to pDD259, except for the C1A mutation in the *Npu*DnaE intein to prevent the initial step (N-S acyl shift) during the protein splicing reaction.
- Co-transformation of pDD260 and pDD261: When the C- and N-terminal domains of the intein are expressed, they should interact to form a functional intein (protein *trans*-splicing, which will therefore be spliced to give rise to the reconstituted functional mCherry protein). Subsequently, in the cells co-transformed with these two plasmids, we should be able to detect mCherry fluorescence upon induction of expression with IPTG and arabinose. Induction with IPTG or arabinose alone, however, should not yield significant amounts of functional mCherry protein.

Questions:

1.  What are the positive and negative controls?
2.  How many conditions do we need to perform in the experiment?

![Figure 17. \*\* Scheme for the protein trans-splicing experiment to design logic gates.](/img/user/figures/inteins_boolean_gates.png)

### Materials

**Table 13.** Materials used in Experiment III.

| Item                        | Composition/Concentration                                                | Application                   |
|-----------------------------|--------------------------------------------------------------------------|-------------------------------|
| Arabinose                   | 20%                                                                      | Induce expression of PBAD     |
| Ampicillin                  | 100 mg/mL                                                                | Selection marker              |
| Kanamycin                   | 50 mg/mL                                                                 | Selection marker              |
| IPTG                        | 1 M                                                                      | Induce expression of PT7      |
| LB-Medium                   | 10 g/L tryptone, 5g/L yeast extract, 10 g/L NaCl, pH 7.0.                | Bacteria growth medium        |
| PBS                         | 2.7 mM KCl, 1.5 mM KH~2~PO~4~, 8.0 mM Na~2~HPO~4~, 137 mM NaCl in dH~2~O | Buffer used for cell diluting |
| *E. coli* T7 express strain |                                                                          | Expresses T7 RNA- polymerase  |

### Protocol

#### Day 6: Transformation of Bacterial Strains

1.  Thaw cells on ice (*E. coli* T7 Express strain).
2.  Add \~1 µL of plasmid DNA (see group distribution below) on top of cells (for co-transformation, add 2 µL each).
3.  Incubate on ice for \~10 min.
4.  Heat shock at 42°C for 45 s.
5.  **Immediately** incubate on ice for 2 min.
6.  Add 250 µL LB-medium.
7.  Shake for \~1 h at 37°C.
8.  Streak out 10 µL (20 µL for co-transformation) on antibiotic-LB-Agar plates (use correct antibiotics!).
9.  Incubate at 37°C overnight.

#### Day 7: Intein Experiment in E. coli

| Plasmid          | Gr. 1 | Gr. 2 | Gr. 3 | Gr. 4 | Gr. 5 | Gr. 6 | Gr. 7 | Gr. 8 |
|------------------|-------|-------|-------|-------|-------|-------|-------|-------|
| pDD259           | I     | I     | \-    | \-    | I     | I     | I     | I     |
| pDD262           | I     | I     | \-    | \-    | \-    | \-    | \-    | \-    |
| pDD260/261       | I/A   | I/A   | I/A   | I/A   | I/A   | I/A   | I/A   | I/A   |
| pDD260/261 (alt) | \-    | \-    | \-    | \-    | I     | I     | A     | A     |

1.  Prepare an Eppendorf tube (1.5 mL) with 50 µL LB-medium and a Falcon tube (15 mL) with 5 mL LB-medium.
2.  Pick \~15 colonies and resuspend in an Eppendorf tube.
3.  Inoculate 5 mL of LB-media (Falcon tube) with 20 µL of cell suspension.
4.  Add antibiotics (AMP = 100 µg/mL, KAN = 50 µg/mL).
5.  Place the Falcon tube into the incubator at 37°C and shake for \~1 h.
6.  Measure OD~600~ nm until \~0.6 (better lower than higher!), follow the bacterial growth by noting the OD values on the white board together with the time of measurement. Analyze the growth curve.
7.  When OD₆₀₀ nm has reached 0.6, induce with IPTG and/or Arabinose (IPTG = 1 mM, Arabinose = 0.04%).
8.  After induction, transfer the Falcon tube into the incubator at RT and shake overnight.

(Optional after 3–4 h: Take \~200 µL of cell suspension and spin down until the pellet is visible).

can you already see a red colored pellet? What does it mean?

#### Day 8: Measurement & Analysis

1.  Spin down Falcon at \~3000 *xg* for 3min.
2.  Discard supernatant and resuspend cells in 5 mL PBS.
3.  Load a transparent 96-well plate with 100 µL of cell suspension, pipette three replicates for each condition.
4.  Measure mCherry fluorescence using the plate reader.
5.  Measure OD~600~ nm on the same plate as the normalization readout.
6.  Determine the mCherry fluorescence of each sample normalized to the cell density (OD~600~ reading). Illustrate the averaged values graphically.


---
[[digital_garden/experiment2\|< Previous: Experiment II]] | [[digital_garden/experiment4\|Next: Experiment IV >]]
