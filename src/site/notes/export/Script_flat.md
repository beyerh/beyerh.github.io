---
{"dg-publish":true,"permalink":"/export/script-flat/","tags":["gardenEntry"]}
---

# Course Information

## Supervisors

Benjamin McLean, Cha San Koh, Daniel Wiebensohn, Dominic Schirmer, Josepha Grewer, Maria Evangelopoulou, Micail David Müller, Miriam Labusch

## Course Materials

Sciebo folder: <https://uni-duesseldorf.sciebo.de/s/KPoKTwFd2jeXfFj>

## Time Schedule

<figure id="fig:schedule-part1" class="align-left" style="width: 100%; display: block; margin-right: auto">

![Figure 1](/img/user/figures/schedule_part1.png)

<figcaption>
<strong>Figure 1.</strong> 
Time Schedule for the first two weeks of the course.
</figcaption>
</figure>
<figure id="fig:schedule-part2" class="align-left" style="width: 100%; display: block; margin-right: auto">

![Figure 2](/img/user/figures/schedule_part2.png)

<figcaption>
<strong>Figure 2.</strong> 
Time Schedule for the third week of the course like in <strong><span
class="citation"
data-cites="Fig:schedule-part1">@Fig:schedule-part1</span></strong>.
</figcaption>
</figure>

## Notes

**Welcome to the course.** We are looking forward to the next two weeks together with you and hope that you enjoy the course content.

**Preparation**

To understand and enjoy all parts of this practical course, it is required that you work through the script before you perform the experiments. The background section serves as a basis for understanding the individual experiments and will be complemented by our lecture series. Your preparations also allow you to read up on topics where you would like to know more, or that still seem confusing to you. Take the opportunity to ask as many questions as you would like during the course. All experiments provide ample room for discussion among students and between students and supervisors.

**Protocol**

Keep constant documentation of your work. You will need all the information for your protocol. The final protocol must include all experimental parts, and they must be introduced scientifically. The protocol must further comprise raw and analyzed results, which should be presented in a comprehensive format (e.g., Tables, Figures, Schemes, etc.) with clear labels. Each experiment requires a discussion of the results. When referencing other works, these must be clearly cited.

**Information on protocols**

Keep constant documentation of your work. You will need all the information for your protocol. The final protocol must include all experimental parts, and they must be introduced scientifically.

The protocol of each part of the experiments should include the following sections:

**1) Goal**

3-10 sentences to describe what you would like to achieve with the experiments.

**2) Method and materials**

Describe suitable approaches you need to perform and reproduce the experiment; materials, including the plasmids, cell types, software, or provided datasets, etc. This part can be brief, as we have detailed lists in the script to which you can refer; however, the differences from the information and protocols outlined in the script must be mentioned.

**3) Procedure and results**

Description of how you have performed the experiments. This part cannot simply refer to the script, as you may modify some of the steps. The results part should show annotated, analyzed data such as labeled gels, plots of measurements including axis titles and error estimates, statistics information, representative images of microscopic data, etc. If any source or dataset was from someone or elsewhere, they should be clearly referenced.

**4) Discussion and conclusion**

The discussion and conclusion parts are based on your analyzed data. Did the result achieve your goals? What have I learned? What went wrong? What should be improved?

**Scope**

Limit the text of each experiment to 1–2 pages (depending on font size and formatting), excluding graphical elements and their captions.

# Background

## Protein Switches

Proteins constitute a group of macro-biomolecules that provide cells with unique functions essential for life. Comprising one or several chains of amino acids, proteins adopt complex 3-dimensional shapes serving as scaffolds for their biological role. Within organisms, proteins act, for example, as biocatalysts involved in cell metabolism or homeostasis (e.g., replication of the genome, energy conversion, protein synthesis, signal propagation). Proteins further provide structure to cells and organisms, engage in intra- and extracellular communication (cell signaling cascades, hormones, receptors and ligands, transporters, etc.), or regulate each other (feedback loops, induction of events such as transcription, translation, polymerization, mobility, etc.). Due to the wide range of different biological functions inherent to natural proteins, they offer unique opportunities for engineering novel protein-based functions, for example, using synthetic biology-inspired approaches.

### Engineered Protein Switches and Optogenetics

Inducible gene expression switches are an example of engineered protein switches. Chemically controlled molecular switches have played a central role in the fundamental study of life, and the emergence of synthetic biology. They have become routine tools in cell biology research and industry (**Figure 3**).

<figure id="fig:tetracycline-switch" class="align-left" style="width: 50%; display: block; margin-right: auto">

![Figure 3](/img/user/figures/tetracycline.png)

<figcaption>
<strong>Figure 3.</strong> 
Tetracycline-inducible gene expression switch based on an engineered
protein switch, the reversed tetracycline transactivator (rtTA). The
engineered “reversed” bacterial repressor protein rTetR binds to a
cognate operator DNA sequence (Tet-response element, TRE) in the
presence of the antibiotic tetracycline. rTetR is fused to a viral
transactivator VP16 which induces gene expression from a minimal
promoter (Pmin) upon DNA binding to induce transcription of a gene of
interest (goi).
</figcaption>
</figure>

> *Note: the natural bacterial tetracycline repressor protein TetR acts as a repressor of transcription in gram-negative bacteria and releases DNA in the presence of tetracycline to induce the expression of resistance genes (TetR, the repressor; and TetA, the protein that pumps antibiotic tetracycline extracellularly).*

However, drawbacks inherent to small molecules like tetracycline, such as difficulties in removing the inducer and diffusion-based transport, have prevented rapid reversibility and spatially-resolved activation. In contrast, light offers unprecedented spatial and temporal resolution. Consequently, the development of light-controlled devices is highly desirable and has recently received much attention, resulting in a variety of different light-controlled tools in bacteria and yeast as well as in mammalian cells. These control diverse cellular activities, including gene expression.

The first light-controlled molecular tools were constructed by introducing photo-cleavable inhibiting chemical groups into inducers, nucleic acids, and transactivators that could be cleaved off in response to UVB light. However, a significant disadvantage of this method is the need to exogenously apply the caged molecules or to reprogram the translation machinery for the incorporation of non-natural amino acids. This disadvantage has been overcome by the optogenetic approach that combines optical and genetic methods to develop light-responsive tools. The first breakthrough in mammalian optogenetics was the discovery of microbial opsins and their subsequent introduction in neuroscience, which revolutionized the study of neuronal networks. Channelrhodopsin, the first opsin that was applied in mammalian neurons, becomes permeable to cations upon blue light illumination, thus triggering neuronal activation. Later, channelrhodopsin was complemented by other ionotropic receptors, including the orange light-responsive, chloride pump halorhodopsin, which made it possible to use dual‑wavelength control to excite or inhibit neurons with subcellular resolution, even in intact brain tissue and in moving animals. Moving beyond neuroscience, more recent optogenetic tools have been engineered to control diverse signaling processes on the protein level in mammalian cells, including gene expression and protein stability, subcellular localization of proteins, receptor and kinase activity, organelle movement, etc. To this end, photoreceptors from all kingdoms of life that naturally sense environmental light information by responding to light of distinct regions of the light spectrum have been employed as engineering scaffolds based on modulating protein-protein interactions, or protein conformation in response to light stimulation (Müller et al., 2015). **Figure 2** illustrates two photoreceptors that are frequently employed in optogenetic protein engineering approaches.

<figure id="fig:photoswitchable-domains" class="align-left" style="width: 100%; display: block; margin-right: auto">

![Figure 4](/img/user/figures/photoswitches.png)

<figcaption>
<strong>Figure 4.</strong> 
<strong>Photoswitchable domains frequently used for optogenetic
engineering. A)</strong> <em>A. thaliana</em> Phytochrome B (PhyB)
photoreceptor. Red light (R) induces a conformational change in PhyB via
a bound linear billin chromophore (not shown), allowing it to
heterodimerize with Phytochrome-Interacting-Factor 6 (PIF6). Far-red
light (FR) induces the dissociation of the PhyB/PIF6 complex.
<strong>B)</strong> Light-Oxygen-Voltage LOV2 domain of <em>Avena
sativa</em> phototropin 1 uses a flavin mononucleotide (FMN, not
illustrated) to sense blue light. Photoexcitation leads to relaxation of
helix Jα, which rewinds in darkness. <em>As</em>LOV2 is often used
either to cage peptides in the dark state (top), or when inserted into
other proteins, to induce structural remodeling upon light treatment
which influences the function of the target protein.
</figcaption>
</figure>

### Protein Splicing

Protein splicing is a natural phenomenon catalyzed by autocatalytic protein domains called inteins (internal proteins). Inteins reside within other proteins, usually close to the active site of proteins, which are essential for the fitness of a given organism. After translation, inteins autocatalytically excise themselves from the precursor protein and covalently ligate the flanking protein sequences (exteins) with a regular peptide bond, a process called protein *cis*-splicing, thereby functionally reconstituting the sequence of the host proteins (**Figure 5**A).

<figure id="fig:protein-splicing" class="align-left" style="width: 100%; display: block; margin-right: auto">

![Figure 5](/img/user/figures/inteins.png)

<figcaption>
<strong>Figure 5.</strong> 
<strong>Protein splicing in <em>cis</em> and <em>trans</em>. A)</strong>
After protein synthesis, protein cis-splicing leads to the
self-catalyzed excision of an intein from a precursor protein and the
covalent ligation of the flanking extein sequences. <strong>B)</strong>
In protein trans-splicing, the association of split intein fragments
(IntN and IntC) initiates reconstitution of the intein and triggers
protein splicing in trans, leading to the ligation of individual
polypeptides.
</figcaption>
</figure>

Little is known about the biological relevance of inteins and therefore, they are mainly seen as selfish genetic elements capable of inserting into protein-encoding genes. Because inteins tend to insert into genes encoding essential proteins with a high degree of conservation, they may be maintained within populations as long as they sufficiently catalyze their self-removal, thereby escaping genetic drifts. However, it seems plausible that some inteins might act as environmental sensors and regulate the activity of their host proteins accordingly (e.g., reduce the growth rate under stress conditions). From genome-mining approaches, split inteins have been identified which can ligate individual polypeptides upon fragment complementation of a N- and C-intein fragment (Int<sub>N</sub> and Int<sub>C</sub>) in a protein trans-splicing reaction (**Figure 5**B). Additionally, one can often engineer *cis*-splicing into *trans*-splicing inteins. Protein *cis*-splicing gave rise to a variety of applications as it allows covalently ligating protein sequences in a solvent-free medium (*in vivo* or *in vitro*) without the requirement of additional cofactors and energy sources. Protein splicing of class 1 inteins, representing the most frequently-found examples, occurs in 4 concerted steps, involving the first intein residue (Cys 1 or Ser 1), the first residue of the C‑terminal extein (Cys/Ser/Thr +1), and the last intein residue (typically Asn) (**Figure 4**).

<figure id="fig:splicing-mechanism" class="align-left" style="width: 70%; display: block; margin-right: auto">

![Figure 6](/img/user/figures/intein_mechanism.png)

<figcaption>
<strong>Figure 6.</strong> 
<strong>Conventional protein splicing mechanism of class 1
inteins.</strong> Step 1: N-S acyl shift of the Cys 1 (in some cases Ser
1) and the N-terminal extein to form a linear thioester. Step 2:
Trans-esterification of Cys +1 (in some cases Ser/Thr +1) to a branched
intermediate where the N- and C-exteins are already covalently connected
and the intein is still attached. Step 3: Asn cyclization into a
succinimide, thereby releasing the intein. Step 4: Spontaneous O-N shift
rearrangement into the energetically-favorable peptide bond (not
intein-catalyzed). Figure modified from Friedel <em>et al.</em>, 2019.
</figcaption>
</figure>

Split inteins in particular found a wide range of applications including their use for protein labeling, protein semi-synthesis, protein purification, protein cyclization, or for engineering protein logic gates. **Figure 7** summarizes some recent examples of developments utilizing split intein technologies (Friedel *et al*., 2019).

<figure id="fig:split-intein-apps" class="align-left" style="width: 100%; display: block; margin-right: auto">

![Figure 7](/img/user/figures/inteins_applications.png)

<figcaption>
<strong>Figure 7.</strong> 
<strong>Applications of split intein technologies.</strong> Bi-specific
antibodies ligated in vitro using split inteins and individual Fab
fragments. <strong>Biosensors</strong> to detect caspases. <em>In
vivo</em> cyclization of the fluorescent protein mNeonGreen2 abolishes
fluorescence. Cleavage of the engineered DEVD sequence by caspases
releases the cyclic tension, resulting in fluorescence. <strong>Gene
therapy</strong> facilitated by individual packaging of two split CRISPR
Cas9 enzyme fragments into adeno associated viral vectors (AAVs),
thereby respecting the viral packaging capacity. Intein trans splicing
reconstitutes the Cas9 enzyme upon co-infection of a target cell with
both vectors.
</figcaption>
</figure>

## AQUA Cloning

The implementation of synthetic biology approaches, for example to the study of cell signaling, demands a wide variety of constructs, including complex combinations of synthetic protein modules, promoters, reporters, etc. The cloning of numerous constructs is time and cost demanding, therefore novel cloning approaches are necessary to simplify the engineering process. One of such methods is AQUA Cloning (**Figure 8**). During the practical part you will be introduced into this technique: Multiple DNA fragments sharing 20-60 bp overlap can easily be assembled into vectors in *E. coli* cells, based on *in vivo* recombination, omitting the need for enzymes commonly mediating the DNA cloning reaction in a test tube. In the practical course you will use a polymerase chain reaction (PCR) and AQUA Cloning as well as conventional restriction and ligation cloning to construct bacterial vectors encoding a split intein-based protein logic gate for an experiment in the following week. At the same time, you will engineer suitable control vectors. The resulting vectors will be analyzed using analytical restriction enzyme digestion and agarose gel electrophoresis, followed by Sanger sequencing.

<figure id="fig:aqua-cloning" class="align-left" style="width: 100%; display: block; margin-right: auto">

![Figure 8](figures/aqua_workflow.png)

<figcaption>
<strong>Figure 8.</strong> 
<strong>AQUA Cloning.</strong> Advanced quick assembly cloning is a
simple yet versatile cloning method (Beyer et al., 2015).
(<strong>a</strong>) DNA parts are produced by PCR, or restriction
digest (or both). Oligonucleotides are designed to contribute flanking
homologous regions to adjacent DNA fragments of optimally 32 bp in
length. DNA parts are assembled into a circular plasmid by
sequence-determined directionality <em>in vivo</em> by <em>E. coli</em>.
(<strong>b</strong>) AQUA Cloning work-flow. (1) DNA parts are generated
by PCR amplification, or derive from an enzymatic digestion. (2) Next,
DNA parts are purified by gel-electrophoresis and (3) mixed and simply
incubated in water prior to transformation into chemically competent
<em>E. coli</em> Top10 cells for <em>in vivo</em> assembly. (4) Finally,
the obtained colonies are confirmed for correct assembly by standard
methods such as analytical PCR, restriction digest, and/or comprehensive
sequencing. {#fig:aqua-cloning}
</figcaption>
</figure>

## Transfection of Mammalian Cells

The process of introducing nucleic acids into mammalian cells by non-viral methods is defined as transfection. By using various chemicals, lipid-based or physical methods, this gene transfer technology is a powerful tool to study gene function and protein expression in the context of a cell. Basically, transfection is a method that overcomes the challenge of introducing molecules with a negative charge (e.g. the phosphate backbone of DNA) into cells with a negatively charged membrane.

Ions like calcium or cationic lipid-based reagents coat the DNA, thus creating an overall positive charge that facilitates uptake of the DNA-transfection reagent complex across the cell membrane (**Figure 9**).

<figure id="fig:transfection-mechanism" class="align-left" style="width: 100%; display: block; margin-right: auto">

![Figure 9](/img/user/figures/transfection.png)

<figcaption>
<strong>Figure 9.</strong> 
<strong>Transfection using chemical reagents. A)</strong> Common
cationic transfection reagents for the generation of reagent: DNA
complexes with a net positive charge. <strong>B)</strong> Overview of
the transfection mechanism. DNA is complexed with the cationic reagent.
The positively charged complexes associate to the negatively charged
membrane and are taken up by endocytosis. Upon escape from the endosome,
the DNA is free to enter the nucleus (e.g., during cell division).
Figure created with BioRender.com
</figcaption>
</figure>

In the practical course polyethylenimine (PEI) will be employed to exemplify transfection using chemical reagents.

PEI is a poly-cationic polymer that is mixed with the DNA in a ratio that ensures the formation of complexes that carry a net positive charge. These cationic complexes interact with the negatively charged cell-surface and are taken up by endocytosis. Inside the endosome, PEI acts as a proton sponge, preventing acidification that is required for the activity of endosomal nucleases (**Figure 10**).

<figure id="fig:pei-transfection" class="align-left" style="width: 100%; display: block; margin-right: auto">

![Figure 10](/img/user/figures/transfection_pei.png)

<figcaption>
<strong>Figure 10.</strong> 
<strong>Polyethyleneimine (PEI)-mediated transfection of mammalian
cells. (a)</strong> Chemical structure <strong>(b)</strong> Mechanism of
PEI-mediated transfection. The positively charged PEI:DNA complexes are
taken up by endocytosis. Inside the endosome PEI prevents acidification,
which eventually leads to rupture of the endosome and liberation of the
DNA into the cytoplasm.
</figcaption>
</figure>

## Genome Engineering of Mammalian Cells

Upon transfection into mammalian cells, nucleic acids can contribute to the genetic programming and instruct cells to execute or alter particular activities. Commonly, either RNA- or DNA-molecules are employed, which in most cases perform their biological function in the cytoplasm and nucleus, respectively. Current RNA-based Covid-19 vaccines, for example, rely on mRNA which upon cell uptake, undergoes ribosomal translation into fragments of the viral spike protein in the cytosol. For the production of biopharmaceuticals and research purposes in cell lines, DNA plasmids are commonly used, which require nuclear entry in order to reach the cell compartment where RNA transcription takes place (**Figure 11**).

<figure id="fig:mammalian-plasmid" class="align-left" style="width: 70%; display: block; margin-right: auto">

![Figure 11](/img/user/figures/mammalian_cell_plasmid.png)

<figcaption>
<strong>Figure 11.</strong> 
Example of a mammalian cell plasmid including mammalian cell-specific,
as well as bacterial features.
</figcaption>
</figure>

Both examples lead to a transient activity of the transfected genetic material. However, over time, the RNA/DNA will be cleared, usually within a time frame of a few days. In rare cases, transfected DNA can integrate at random positions into the cell genome (roughly in 1 out of 1.000 transfected cells, strongly depending on the cell, construct, and the exact experimental conditions). By using additional eukaryotic antibiotic resistance genes encoded on the transfected plasmid, one can positively select for these cells. During the past years, several methods have been developed that facilitate the targeted integration of genetic material into mammalian cells or the specific alteration of the cellular genomes. During the theoretical parts of the course, you will have the possibility to familiarize yourself with some examples spanning this topic. Methods to integrate genetic information into cell genomes for example rely on (i) the above-mentioned random DNA integration, (ii) viral gene vehicles, e.g. using lentiviral systems harboring reverse transcriptases and integrases, (iii) homologous recombination-based techniques including the use of recombinases or designer endonucleases and homology templates containing the desired genetic information, or (iv) transposase-technologies originating from transposons (“jumping genes”) which excise and integrate genetic information. Table **Table 1** summarizes particular properties of these four groups.

Experiment II of this practical course will introduce you to a blue light-sensitive optogenetic gene expression system. Here, you will use mammalian cells that have genomic integrations for the required optogenetic switches and the target gene, which will be expressed upon stimulation with light. These cells were generated using the Sleeping Beauty SB100X transposase, as explained in **Figure 12**. “Sleeping Beauty” refers to a transposase that was originally identified as an inactive enzyme in salmonid fish. Targeted mutagenesis, however, restored the activity after a long evolutionary sleep, and rounds of directed evolution finally yielded a hyperactive transposase enzyme, which is nowadays widely used for genome engineering purposes (Mátés et al., 2009).

<figure id="fig:sleeping-beauty" class="align-left" style="width: 80%; display: block; margin-right: auto">

![Figure 12](/img/user/figures/transposases.png)

<figcaption>
<strong>Figure 12.</strong> 
<strong>Mode of function of SB100X Sleeping Beauty-catalyzed
transposition.</strong> Cotransfection of plasmids (i) containing a
genetic cargo which is flanked by inverted terminal repeats (ITRs), and
(ii) a transiently-expressed SB100X transposase gene leads to
transposition of the cargo into the cell genome. SB100X excises the
genetic cargo from the plasmid and integrates it at random positions (TA
sites) into the host genome. Abbreviations: GOI, gene of interest; P,
promoter; Res, resistance gene.
</figcaption>
</figure>
<figure id="tbl:integration-methods" class="align-left" style="width: 100%; float: left; margin-right: 1em">
  <figcaption>
    <strong>Table 1.</strong> 

  </figcaption>
<table>
<colgroup>
<col style="width: 22%" />
<col style="width: 38%" />
<col style="width: 28%" />
<col style="width: 12%" />
</colgroup>
<thead>
<tr>
<th>Technology</th>
<th>Advantages</th>
<th>Drawbacks</th>
<th>Additional Info</th>
</tr>
</thead>
<tbody>
<tr>
<td>Random integration</td>
<td>No additional components required other than selection.</td>
<td>Very inefficient. Random integration sites.</td>
<td></td>
</tr>
<tr>
<td>Lentiviral delivery</td>
<td>Highly efficient, <em>in vitro</em> and <em>in vivo</em>
applications possible.</td>
<td>Complex protocol including viral particle generation, eventually S2
biosafety level. Random integration sites. Size limited by viral
packaging capacity.</td>
<td>Multiple insertions likely.</td>
</tr>
<tr>
<td>Recombination-based integration</td>
<td>Targeted</td>
<td></td>
<td></td>
</tr>
<tr>
<td>Transposase-based integration</td>
<td>As efficient as lentiviral systems but under S1 biosafety level. No
size limitation of transposed genes.</td>
<td>Random integration.</td>
<td></td>
</tr>
</tbody>
</table>
</figure>

## Mammalian Cell Lines Used in This Course

<figure id="tbl:cell-lines" class="align-left" style="width: 100%; float: left; margin-right: 1em">
  <figcaption>
    <strong>Table 2.</strong> 

  </figcaption>
<table>
<colgroup>
<col style="width: 20%" />
<col style="width: 40%" />
<col style="width: 40%" />
</colgroup>
<thead>
<tr>
<th>Name</th>
<th>Description</th>
<th>Cultivation</th>
</tr>
</thead>
<tbody>
<tr>
<td>CHO-K1</td>
<td>Subclone from parental CHO cell line that was initiated from an
ovary biopsy of an adult Chinese hamster in 1957.</td>
<td>90% Ham’s F12 + 10% h.i. FBS</td>
</tr>
<tr>
<td>HeLa</td>
<td>Human cervix carcinoma cells.<br><br>Established from the epitheloid
cervix carcinoma of a 31-year-old woman in 1951; later diagnosis changed
to adenocarcinoma</td>
<td>DMEM medium, completed with 10% FCS and 1 %
Penicillin/Streptomycin</td>
</tr>
</tbody>
</table>
</figure>

# Practical Part

## Experiment I: Molecular Cloning of Bacterial Inducible Plasmids

**Supervisors:** Alexander Geidies, Cha San Koh, Maria Medar, Sara Shumka, Daniel Wiebensohn

alexander.geidies@hhu.de, koh@hhu.de, marija.medar@hhu.de, sara.shumka@uni-duesseldorf.de, daniel.wiebensohn@uni-duesseldorf.de

Constructing recombinant genes within plasmids facilitates their recovery, genetic engineering *ex-vivo*, and shuttling into different desired strains or hosts. Recombinant DNA technologies represent the foundation for generating constitutive or inducible expression systems for the study of heterologous genes in different systems of interest.

In this first experimental part, we will design the required vectors for Experiment III, the design of protein logic gates based on protein *trans*-splicing in bacteria. For this purpose, we will use two different molecular DNA cloning techniques: 

A. Restriction and ligation cloning. This technique relies on the presence of restriction enzyme (dE) recognition sites flanking the desired insert and as well as at the desired positions in the recipient plasmid. The REs will then generate double DNA cuts leaving cohesive or blunt ends in both DNA sequences, in two independent reactions. Afterwards, we will purify the digested fragments and ligate them together using an enzyme called T4 DNA ligase, before transformation into chemically competent *E. coli* TOP10 bacteria for subsequent amplification and selection. T4 DNA ligase will conduct the repair of the broken DNA by forming a phosphodiester bond between a nearby 5’‑phosphate and 3’-OH ends resulting in the assembly of the desired new vector (**Figure 12**).

B. Advanced Quick Assembly (AQUA) Cloning. In contrast to conventional restriction/ligation cloning, this technique allows us to design a vector independently of the presence of suitable RE sites or the use of DNA restriction enzymes and ligases. This versatile and inexpensive technique relies on *in-vivo* DNA recombination within *E. coli* and therefore, requires DNA fragments that share an overlapping region of 20-60 bp at the junction sites. The homology region can for example be generated by PCR using appropriate primers that add these sequences to the products (**Figure 12**). AQUA Cloning can also be used to clone multiple DNA fragments simultaneously, reminiscent to other “DNA assembly cloning” methods. Additionally, a combination of restriction of the backbone and PCR amplification of the insert (as we will see in our exercise) can be used.

Each group will perform one ligation and one AQUA cloning experiment from one of the four plasmids:

- Groups 1 and 2: pDD259.
- Groups 3 and 4: pDD260.
- Groups 5 and 6: pDD261.
- Groups 7 and 8: pDD262.

As outlined in **Figure 12**, we will first perform a PCR reaction to amplify: a. The gene encoding the fluorescent protein mCherry interrupted by the full-length *Npu*DnaE intein gene (Int); b. The mCherry gene was disrupted by a mutated (non-functional) version of the intein; c. A DNA fragment encoding an N-terminal portion of mCherry (mChN) fused to an N-terminal split-fragment of the intein (IntN); and d. a DNA fragment encoding a C-terminal portion of mCherry (mChC) fused to a C-terminal split-fragment of the intein (IntC). The destination vectors will be digested overnight with the annotated restriction enzymes to generate the so-called vector “backbones” (this step will be performed by the supervisors in advance).

After gel purification of the PCR products, we will need to digest the PCR product with the same enzymes as the destination vectors in order to clone the genes via ligation cloning. We will then prepare a pre-mix with a 3:1 ratio of the corresponding fragments (insert:backbone). For the restriction/ligation protocol, remember to add T4 DNA ligase and the corresponding buffer! After ligation, the DNA mixtures will be transformed into competent Top10 *E. coli* cells and plated on LB agar plates containing the appropriate antibiotics for selection of transformed cells.

The engineered vectors will be purified and analyzed using analytical restriction enzyme digestion and agarose gel electrophoresis. We encourage you to consider beforehand which enzymes we could use to differentiate the restriction pattern expected for the original plasmids and that resulting from the digestion of the engineered vectors.

Finally, we will select some promising samples and analyze them by Sanger sequencing.

<figure id="fig:cloning-strategy" class="align-left" style="width: 100%; display: block; margin-right: auto">

![Figure 13](/img/user/figures/cloning_strategies.png)

<figcaption>
<strong>Figure 13.</strong> 
<strong>Illustration of the cloning strategy.</strong> Top, schematic
representation of the cloned vectors. Bottom, pRSFDuet-1 plasmid (KanR)
digested with <em>Bam</em>HI and <em>Kpn</em>I serves as backbone for
cloning plasmids pDD259/262 and 260. The inserts for these constructs
are the amplification products of pDD002 and pDD083 with the primers
oDD561 and oDD562; or the PCR product of pDD002 with oDD561 and oDD563,
respectively.
</figcaption>
</figure>

A third insert amplified from pDD002 with the primer oDD564 and oDD565 will be cloned into pHBBAD090 backbone, previously digested with *Nde*I and *Hin*dIII, to obtain pDD261. The primers were designed so that the PCR products possess the required homology regions to the digested vector backbones for AQUA Cloning. Alternatively, the PCR products can be digested using the indicated enzymes for ligation cloning. Both approaches result in the same final vectors.The \* symbol represents the location of the C1A mutation in the pDD262.

### Materials

<figure id="tbl:materials-exp1" class="align-left" style="width: fontsize; float: left; margin-right: 1em">
  <figcaption>
    <strong>Table 3.</strong> 

  </figcaption>
<table>
<colgroup>
<col style="width: 16%" />
<col style="width: 18%" />
<col style="width: 42%" />
<col style="width: 8%" />
<col style="width: 16%" />
</colgroup>
<thead>
<tr>
<th>Category</th>
<th>Item</th>
<th>Composition</th>
<th>Conc.</th>
<th>Use</th>
</tr>
</thead>
<tbody>
<tr>
<td><strong>Plasmids</strong></td>
<td>pRSFDuet-1</td>
<td>PT7-H6-MCS-term (KanR)</td>
<td></td>
<td>Digested backbone</td>
</tr>
<tr>
<td></td>
<td>pDD002</td>
<td>PSV40-mCherryN-Int-mCherryC-pA (AmpR)</td>
<td></td>
<td>PCR template</td>
</tr>
<tr>
<td></td>
<td>pHBBAD090</td>
<td>PBAD-Insert-term (AmpR)</td>
<td></td>
<td>Digested backbone</td>
</tr>
<tr>
<td></td>
<td>pDD083</td>
<td>PSV40-mCherryN-Int(C1A)-mCherryC-pA (AmpR)</td>
<td></td>
<td>PCR template</td>
</tr>
<tr>
<td><strong>Primers</strong></td>
<td>oDD561</td>
<td>5’-AGCAGCCATCACCATCATCACCACAGCCAG-GATCCGGTGAGCAAGGGCGAGGAG</td>
<td>25 µM</td>
<td>mCh F <em>Bam</em>HI duet</td>
</tr>
<tr>
<td></td>
<td>oDD562</td>
<td>5’-GCAGCAGCGGTTTCTTTACCAGACTCGAGGG-TACCTTACTTGTACAGCTCGTCCATGC</td>
<td>25 µM</td>
<td>mCh R <em>Kpn</em>I duet</td>
</tr>
<tr>
<td></td>
<td>oDD563</td>
<td>5’-GCAGCAGCGGTTTCTTTACCAGACTCGAGGG-TACCTTAATTCGGCAAATTATCAACCCGC</td>
<td>25 µM</td>
<td>NpuEN R <em>Kpn</em>I duet</td>
</tr>
<tr>
<td></td>
<td>oDD564</td>
<td>5’-TGTTTAACTTTAAGAAGGAGATATACATATG-ATCAAATAGCCACACGTAAATATTTAGG</td>
<td>25 µM</td>
<td>NpuE_C F <em>Nde</em>I bad</td>
</tr>
<tr>
<td></td>
<td>oDD565</td>
<td>5’-AAAATCTTCTCTCATCCGCCAAAACAGCCA-AGCTTACTTGTACAGCTCGTCCATGC</td>
<td>25 µM</td>
<td>mCh R <em>Hind</em>III bad</td>
</tr>
<tr>
<td><strong>PCR reaction</strong></td>
<td>Q5® High-Fidelity DNA polymerase (NEB)</td>
<td></td>
<td>2,000 U/mL</td>
<td></td>
</tr>
<tr>
<td></td>
<td>Q5 Reaction buffer (5x)</td>
<td>2 mM MgCl<span class="math inline"><sub>2</sub></span></td>
<td>5X</td>
<td></td>
</tr>
<tr>
<td></td>
<td>dNTPs</td>
<td>dATP, dCTP, dGTP and dTTP</td>
<td>10 mM each</td>
<td></td>
</tr>
<tr>
<td><strong>Digestion reaction</strong></td>
<td>Cutsmart (10x) (NEB)</td>
<td>50 mM potassium acetate, 20 mM Tris-acetate, 10 mM magnesium
acetate, 100 μg/mL BSA</td>
<td>10X</td>
<td></td>
</tr>
<tr>
<td></td>
<td>Restriction enzymes (NEB)</td>
<td>selected during the course</td>
<td>3,333 U/mL</td>
<td></td>
</tr>
<tr>
<td><strong>Gel electrophoresis</strong></td>
<td>Agarose</td>
<td></td>
<td></td>
<td></td>
</tr>
<tr>
<td></td>
<td>TE Buffer</td>
<td>10 mM Tris-Cl pH 7.5, 1 mM EDTA</td>
<td></td>
<td></td>
</tr>
<tr>
<td></td>
<td>Gelred</td>
<td></td>
<td></td>
<td>Intercalation agent</td>
</tr>
<tr>
<td></td>
<td>Loading buffer</td>
<td>50% Glycerol, 100 mM Na<span
class="math inline"><sub>2</sub></span>EDTA, pH 8.0, 1% SDS, 0.1%
Bromophenol Blue, 0.1% Xylene Cyanol</td>
<td>6X</td>
<td></td>
</tr>
<tr>
<td></td>
<td>1 Kb DNA ladder</td>
<td></td>
<td></td>
<td>Ladder for 100 bp up to 10 kb</td>
</tr>
<tr>
<td><strong>M.-Nagel Gel extraction</strong></td>
<td>NT1 Buffer</td>
<td></td>
<td></td>
<td>Binding buffer</td>
</tr>
<tr>
<td></td>
<td>NT3 Buffer</td>
<td></td>
<td></td>
<td>Wash buffer</td>
</tr>
<tr>
<td></td>
<td>M&amp;N spin columns</td>
<td></td>
<td></td>
<td>DNA binding</td>
</tr>
<tr>
<td><strong>Ligation</strong></td>
<td>T4 Ligase Buffer (NEB)</td>
<td>300 mM Tris-HCl (pH 7.8), 100 mM MgCl<span
class="math inline"><sub>2</sub></span>, 100 mM DTT, 10 mM ATP</td>
<td>10X</td>
<td></td>
</tr>
<tr>
<td></td>
<td>T4 DNA-ligase (NEB)</td>
<td></td>
<td>400,000 U/mL</td>
<td></td>
</tr>
<tr>
<td><strong>Wizard mini-prep kit</strong></td>
<td>W1</td>
<td>50 mM Tris-HCl (pH 7.5), 10 mM EDTA, 100 μg/mL RNase A</td>
<td></td>
<td>Resuspension solution</td>
</tr>
<tr>
<td></td>
<td>W2</td>
<td>0.2 M NaOH, 1% SDS</td>
<td></td>
<td>Lysis solution</td>
</tr>
<tr>
<td></td>
<td>W3</td>
<td>4.09 M guanidine hydrochloride, 0.759 M potassium acetate, 2.12 M
glacial acetic acid</td>
<td></td>
<td>Neutralization solution</td>
</tr>
<tr>
<td></td>
<td>W4</td>
<td>60% ethanol, 60 mM potassium acetate, 8.3 mM Tris-HCl, 0.04 mM
EDTA</td>
<td></td>
<td>Wash solution</td>
</tr>
<tr>
<td></td>
<td>Wizard columns</td>
<td></td>
<td></td>
<td>DNA purification</td>
</tr>
<tr>
<td><strong>Others</strong></td>
<td>ddH<span class="math inline"><sub>2</sub></span>O</td>
<td></td>
<td></td>
<td></td>
</tr>
<tr>
<td></td>
<td>LB media</td>
<td></td>
<td></td>
<td>Bacteria growth media</td>
</tr>
<tr>
<td></td>
<td>LB-plates with ampicillin</td>
<td></td>
<td>100 μg/mL Amp</td>
<td></td>
</tr>
<tr>
<td></td>
<td>LB-plates with kanamycin</td>
<td></td>
<td>50 μg/mL Kan</td>
<td></td>
</tr>
<tr>
<td></td>
<td>Top10 Invitrogen™</td>
<td>Chemically competent <em>E. coli</em> cells</td>
<td></td>
<td></td>
</tr>
</tbody>
</table>
</figure>

### Protocols

#### Day 1

##### 1.1 PCR

<figure id="tbl:pcr-mixture" class="align-left" style="width: 100%; float: left; margin-right: 1em">
  <figcaption>
    <strong>Table 4.</strong> 
PCR mixture.
  </figcaption>
<table>
<thead>
<tr>
<th>Component</th>
<th>Amount</th>
<th>Unit</th>
</tr>
</thead>
<tbody>
<tr>
<td>Q5 Reaction Buffer</td>
<td>10</td>
<td>µL</td>
</tr>
<tr>
<td>Primer 1, 25 µM</td>
<td>1</td>
<td>µL</td>
</tr>
<tr>
<td>Primer 2, 25 µM</td>
<td>1</td>
<td>µL</td>
</tr>
<tr>
<td>dNTPs, 10 mM</td>
<td>1</td>
<td>µL</td>
</tr>
<tr>
<td>Template DNA</td>
<td>1</td>
<td>µL</td>
</tr>
<tr>
<td>Q5 DNA polymerase</td>
<td>0.5</td>
<td>µL</td>
</tr>
<tr>
<td>add dH<span class="math inline"><sub>2</sub></span>O</td>
<td>32.5</td>
<td>µL</td>
</tr>
<tr>
<td><strong>Total</strong></td>
<td><strong>50</strong></td>
<td><strong>µL</strong></td>
</tr>
</tbody>
</table>
</figure>
<figure id="tbl:primers-templates" class="align-left" style="width: 100%; float: left; margin-right: 1em">
  <figcaption>
    <strong>Table 5.</strong> 
Primers and templates.
  </figcaption>
<table>
<thead>
<tr>
<th>PCR</th>
<th>Forward primer</th>
<th>Reverse primer</th>
<th>Template</th>
<th>Product size (bp)</th>
<th>Ta</th>
</tr>
</thead>
<tbody>
<tr>
<td>PCR259 (pDD259)</td>
<td>oDD561</td>
<td>oDD562</td>
<td>pDD002</td>
<td>ca. 1190</td>
<td>TBD</td>
</tr>
<tr>
<td>PCR262 (pDD262)</td>
<td>oDD561</td>
<td>oDD562</td>
<td>pDD083</td>
<td>ca. 1190</td>
<td>TBD</td>
</tr>
<tr>
<td>PCR260 (pDD260)</td>
<td>oDD561</td>
<td>oDD563</td>
<td>pDD002</td>
<td>ca. 803</td>
<td>TBD</td>
</tr>
<tr>
<td>PCR261 (pDD261)</td>
<td>oDD564</td>
<td>oDD565</td>
<td>pDD002</td>
<td>ca. 454</td>
<td>TBD</td>
</tr>
</tbody>
</table>
</figure>
<figure id="tbl:pcrprogram" class="align-left" style="width: 100%; float: left; margin-right: 1em">
  <figcaption>
    <strong>Table 6.</strong> 
PCR program
  </figcaption>
<table>
<thead>
<tr>
<th>Temperature</th>
<th>Time</th>
<th>Cycles</th>
<th></th>
</tr>
</thead>
<tbody>
<tr>
<td>98°C</td>
<td>5 min</td>
<td>1×</td>
<td></td>
</tr>
<tr>
<td>98°C</td>
<td>30 s</td>
<td>25×</td>
<td></td>
</tr>
<tr>
<td>Ta°C</td>
<td>30 s</td>
<td>25×</td>
<td></td>
</tr>
<tr>
<td>72°C</td>
<td>40 s/kb</td>
<td>25×</td>
<td></td>
</tr>
<tr>
<td>72°C</td>
<td>10 min</td>
<td>1×</td>
<td></td>
</tr>
<tr>
<td>4°C</td>
<td>Hold</td>
<td>-</td>
<td></td>
</tr>
</tbody>
</table>
</figure>

##### 1.2 DNA Purification from Agarose Gel

1.  Agarose-gel electrophoresis: 0.8% agarose in TE Buffer, 1:10,000 Gelred Stock solution (Caution! DNA dyes intercalate, thus are mutagenic agents. Handle it with care).
2.  Sample preparation: Mix 50 µL plasmid DNA with 10 µL of 6x loading buffer.
3.  Use 12 µL DNA-Ladder (MM).
4.  Run gel at 120 V for 20–30 min.

<figure id="fig:dna-ladder" class="align-left" style="width: 30%; display: block; margin-right: auto">

![Figure 14](/img/user/figures/dna_ladder.png)

<figcaption>
<strong>Figure 14.</strong> 
<strong>GeneRuler™ 1 kb DNA Ladder</strong> (Fermentas)
</figcaption>
</figure>

##### 1.3 DNA Purification

1.  Cut bands from the gel and transfer each gel slice into a 1.5 mL tube.
2.  Add approx. 200 µL NTI buffer / 100 mg gel and incubate the tube at 60°C, 200 rpm for \~ 10 min until the gel slice is completely dissolved.
3.  Add the samples onto M&N spin columns, 1 column per gel slice.
4.  Centrifuge at max speed for 60 s at RT and discard the flow through.
5.  Apply remaining sample volumes (if any).
6.  Centrifuge at max speed for 60 s at RT and discard flow-through.
7.  Add 700 µL NT3 buffer to the spin column.
8.  Centrifuge at max speed for 60 s at RT and discard flow through.
9.  Add 700 µL of NT3 buffer to the spin column as an additional washing step.
10. Centrifuge at max speed for 60 s at RT and discard flow through.
11. Centrifuge at max speed for 60 s at RT again and discard flow-through! (To dry the column and remove residual EtOH).
12. Place the column into a fresh and labelled 1.5 mL tube.
13. Add 20 µL ddH~2~O to the column
14. Incubate for 5 min at 70°C.
15. Centrifuge at max speed for 90 s at RT.
16. **KEEP** the flow through, it contains your purified DNA, determine the concentration using the Nanodrop.
17. Store at -20°C.

##### 1.4 Backbone Digestion (Performed by the Supervisors)

<figure id="tbl:digest_bb" class="align-left" style="width: 100%; float: left; margin-right: 1em">
  <figcaption>
    <strong>Table 7.</strong> 
Digestion of vector backbone.
  </figcaption>
<table style="width:70%;">
<colgroup>
<col style="width: 25%" />
<col style="width: 45%" />
</colgroup>
<thead>
<tr>
<th>Component</th>
<th>Volume</th>
</tr>
</thead>
<tbody>
<tr>
<td>Plasmid DNA (2 µg)</td>
<td>x µL</td>
</tr>
<tr>
<td>Cut Smart buffer (10x)</td>
<td>5 µL</td>
</tr>
<tr>
<td>Enzyme 1</td>
<td>2.5 µL</td>
</tr>
<tr>
<td>Enzyme 2</td>
<td>2.5 µL</td>
</tr>
<tr>
<td>CIP (only for the ligation backbone)</td>
<td>1 µL</td>
</tr>
<tr>
<td>H<span class="math inline"><sub>2</sub></span>O</td>
<td>x µL</td>
</tr>
<tr>
<td><strong>Total</strong></td>
<td><strong>50 µL</strong></td>
</tr>
</tbody>
</table>
</figure>

- Incubate ON at 37°C.

We will provide you with the digested destination vectors.

##### 1.5 PCR Products Digestion (Only for Ligation Cloning)

This step will only be performed by the group member doing ligation cloning.

<figure id="tbl:pcr_digest" class="align-left" style="width: 100%; float: left; margin-right: 1em">
  <figcaption>
    <strong>Table 8.</strong> 
Digestion of PCR products.
  </figcaption>
<table style="width:70%;">
<colgroup>
<col style="width: 25%" />
<col style="width: 45%" />
</colgroup>
<thead>
<tr>
<th>Component</th>
<th>Volume</th>
</tr>
</thead>
<tbody>
<tr>
<td>PCR product</td>
<td>23 µL</td>
</tr>
<tr>
<td>Cut Smart buffer (10x)</td>
<td>3 µL</td>
</tr>
<tr>
<td>Enzyme 1</td>
<td>2 µL</td>
</tr>
<tr>
<td>Enzyme 2</td>
<td>2 µL</td>
</tr>
<tr>
<td>H<span class="math inline"><sub>2</sub></span>O</td>
<td>0 µL</td>
</tr>
<tr>
<td><strong>Total</strong></td>
<td><strong>30 µL</strong></td>
</tr>
</tbody>
</table>
</figure>

- Incubate ON at 37°C.

#### Day 2

##### 2.1 Digested PCR Products Purification (Only for Ligation Cloning)

1.  Add approx. 60 µL NTI buffer.
2.  Add the samples onto M&N spin columns, 1 column per digestion.
3.  Centrifuge at max speed for 60 s at RT and discard the flow through.
4.  Apply remaining sample volumes (if any).
5.  Centrifuge at max speed for 60 s at RT and discard flow-through.
6.  Add 700 µL NT3 buffer to the spin column.
7.  Centrifuge at max speed for 60 s at RT and discard flow through.
8.  Add 700 µL of NT3 buffer to the spin column as an additional washing step.
9.  Centrifuge at max speed for 60 s at RT and discard flow through.
10. Centrifuge at max speed for 60 s at RT again and discard flow through! (To dry the column and remove residual EtOH).
11. Place the column into a fresh and labelled 1.5 mL tube.
12. Add 20 µL ddH~2~O to the column
13. Incubate 5 min at 70°C.
14. Centrifuge at max speed for 90 s at RT.
15. **KEEP** the flow through, it contains your purified DNA, determine the concentration using the Nanodrop.

##### 2.2 Assembly of the New Vector

###### 2.2.1 AQUA Cloning

If possible, use approximately 35 ng of DNA for the backbone.

Calculations for the amount of PCR-DNA needed for a 1:3 ratio:

<figure id="tbl:digest" class="align-left" style="width: 100%; float: left; margin-right: 1em">
  <figcaption>
    <strong>Table 9.</strong> 
<strong>Sample 1, Sample 2 (negative control)</strong>
  </figcaption>
<table style="width:70%;">
<colgroup>
<col style="width: 25%" />
<col style="width: 45%" />
</colgroup>
<thead>
<tr>
<th>Component</th>
<th>Volume</th>
</tr>
</thead>
<tbody>
<tr>
<td>Digested backbone</td>
<td>x µL</td>
</tr>
<tr>
<td>PCR product</td>
<td>x µL</td>
</tr>
<tr>
<td>H<span class="math inline"><sub>2</sub></span>O</td>
<td>x µL</td>
</tr>
<tr>
<td><strong>Total</strong></td>
<td><strong>10 µL</strong></td>
</tr>
</tbody>
</table>
</figure>

- Incubate at RT for 60 min.
- Put samples on ice, 5 min.

###### 2.2.2 Ligation Protocol

<figure id="tbl:ligation" class="align-left" style="width: 100%; float: left; margin-right: 1em">
  <figcaption>
    <strong>Table 10.</strong> 
DNA ligation
  </figcaption>
<table style="width:70%;">
<colgroup>
<col style="width: 25%" />
<col style="width: 45%" />
</colgroup>
<thead>
<tr>
<th>Component</th>
<th>Volume</th>
</tr>
</thead>
<tbody>
<tr>
<td>Vector (30-50 ng)</td>
<td>x µL</td>
</tr>
<tr>
<td>Insert (3x excess)</td>
<td>y µL</td>
</tr>
<tr>
<td>H<span class="math inline"><sub>2</sub></span>O (qsf 20 µL)</td>
<td>z µL</td>
</tr>
<tr>
<td>T4 DNA ligase Buffer 10x</td>
<td>2 µL</td>
</tr>
<tr>
<td>T4 DNA ligase</td>
<td>1 µL</td>
</tr>
<tr>
<td><strong>Total</strong></td>
<td><strong>20 µL</strong></td>
</tr>
</tbody>
</table>
</figure>

- Incubate at RT for 60 min.
- Heat inactivate the T4 DNA ligase by incubating 10 min at 65 °C.

##### 2.3 Transformation into *E. coli* Competent Cells

1.  AQUA/Ligation mixture and Negative control mixture
2.  Thaw cells on ice. Carefully add AQUA mix/ negative control (10 µL) or ligation mix/negative control (5 µL). Do not resuspend, just slightly stir using the pipette tip.
3.  Incubate for 30 min on ice, heat-shock for 45 s at 42°C, place on ice for 2 min, add 250 µL LB‑medium and incubate for 1 h at 37°C, 550 rpm.
4.  Finally, plate cells on ampicillin (100 µg/mL) or kanamycin (50 µg/mL) LBagar plates. For the AQUA plate 250 µL/plate and for ligation 100 µL/plate. (In this way, one may ensure the convenient isolation of colonies the next day).
5.  Distribute cells uniformly on the plates.
6.  Incubate plates overnight at 37°C.

#### Day 3

##### 3.1 Streaking Single Colonies on New LB-Ampicillin Plates

- Pick 4 single clones and streak out onto LB plates with ampicillin (100 μg/mL) or kanamycin (50 μg/mL). Streak 2 colonies in each plate. Incubate overnight at 37°C. Make sure to evenly spread the picked colony over the **whole surface** of the LB agar plate.

#### Day 4

##### 4.1 Plasmid DNA Isolation

1.  Using a sterile inoculating loop, scrape bacteria off the plate and resuspend in 250 μL of Cell Resuspension Solution (W1).
2.  Add 250 μL of Cell Lysis Solution (W2) to each sample; **invert** 4 times to mix.
3.  Incubate for 5 min at RT.
4.  Add 350 μL of Neutralization Solution (W3); **invert** 4–6 times to mix.
5.  Centrifuge at max speed for 8 min at RT.
6.  During the centrifugation insert spin columns into collection tubes.
7.  Equilibrate columns with 700 µL ddH~2~O, centrifuge for 60 s at max speed and discard the flow‑through.
8.  After centrifugation, transfer cleared lysates into spin columns.
9.  Centrifuge at max speed for 60 s at RT.
10. Discard flow-through and reinsert columns into collection tubes.
11. Add 750 μl of Wash Solution (WW). Centrifuge at top speed for 60 s. Discard flow-through and reinsert the column into the collection tube.
12. Repeat the previous step with 250 μl of Wash Solution (WW).
13. Centrifuge at max speed for 60 s at RT.
14. Transfer Spin Column into a sterile 1.5 mL tube.
15. Add 60 μl of prewarmed MilliQ-Water to the Spin Column and incubate for 4 min at RT. Centrifuge at max speed for 90 s at RT and **KEEP** the tube with the flow through.
16. Store extracted plasmids at -20°C.
17. Wash the mini column four times with 700 µl of ddH~2~O and keep them. Do not throw them away.

##### 4.2 Analytical Restriction Enzyme Digestion

For each clone, perform one digest of 5 µL as follows:

<figure id="tbl:testdigest" class="align-left" style="width: 100%; float: left; margin-right: 1em">
  <figcaption>
    <strong>Table 11.</strong> 
Test digestion.
  </figcaption>
<table style="width:70%;">
<colgroup>
<col style="width: 25%" />
<col style="width: 45%" />
</colgroup>
<thead>
<tr>
<th>Component</th>
<th>Volume</th>
</tr>
</thead>
<tbody>
<tr>
<td>Plasmid DNA</td>
<td>4 µL</td>
</tr>
<tr>
<td>Cut Smart buffer (10x)</td>
<td>0.5 µL</td>
</tr>
<tr>
<td>Enzyme 1</td>
<td>0.25 µL</td>
</tr>
<tr>
<td>Enzyme 2</td>
<td>0.25 µL</td>
</tr>
<tr>
<td><strong>Total</strong></td>
<td><strong>5 µL</strong></td>
</tr>
</tbody>
</table>
</figure>

1.  Incubate at 37°C for 1–2 h.
2.  Analyze your digest via Agarose-gel electrophoresis: 1% agarose in TE Buffer, 1:10000 Gelred Stock solution (Caution! DNA dyes intercalate, thus are mutagenic agents. Handle it with care).
3.  Sample preparation: Mix 5 µL digest with 1–2 µL of 6× loading buffer.
4.  Run gel 120 V, 20–30 min. Perform graphical analysis of gel.

##### 4.3 Sequencing

Selection of positive colonies.

Send a 12 µL aliquot with a concentration of 40–100 ng/µL. Dilute if necessary.

## Experiment II: Optogenetic Gene Expression Using Stably-Engineered Mammalian Cells

**Supervisors** Maria Medar, David Mohr, Sara Shumka

marija.medar@hhu.de, david.mohr@hhu.de, sara.shumka@uni-duesseldorf.de

The objective of this experiment is to learn how to control and analyze the induction of gene expression via an optogenetic tool in mammalian cells. To this end, foreign genes encoding the photo-switch and a light-inducible reporter encoding a gene of interest were previously introduced into the genome of Chinese Hamster Ovary (CHO-K1) cells. We will treat this customized cell line with light and dark and quantify the reporter expression over a time course of 24 hours.

Transient transfection is an efficient method for preliminary reporter assays. CHO-K1 cells normally achieve high transfection rates and express recombinant proteins in large scale when using polyethylenimine (PEI)-based transient transfection methods (see introduction **Figure 7**). In contrast to many commercial transfection agents, PEI is inexpensive yet very efficient for a range of mammalian cell lines. However, the transfection efficiency can be affected by various parameters (cell type, number of plasmids, DNA amount, DNA quality, etc.). Additionally, in transiently transfected cells, the foreign DNA rarely integrates into the host genome and consequently does not replicate, leading to an eventual loss through cycles of cell division over several days.

Stable genomic integration is often the preferred option as the foreign gene becomes part of the genome which allows for greater process consistency and long-term protein expression. However, the generation of stable cell lines is a time-consuming and expensive process. In this experiment, we will provide a stably-engineered CHO-K1 cell line generated using a sequential genomic integration of two vectors (**Figure 15**). One vector encodes an optogenetic LOVpep/ePDZ-based split transcription factor system under the selection of puromycin, and the other a SEAP reporter under the selection of Hygromycin. The principle of generating stable cell lines using the Sleeping Beauty transposase is explained in the introduction part (**Figure 12**).

The following experiment will be about handling mammalian cell culture as well as the analysis of a light-induced reporter gene. The human placental **se**creted **a**lkaline **p**hosphatase (SEAP) as a reporter has tremendous advantages. SEAP is very stable, and its secretion into the medium allows a convenient and non-invasive way of acquiring samples. Furthermore, it is a quantitative reporter for gene expression because the SEAP activity in the supernatant of transfected CHO-K1 cells is proportional to shifts in intracellular SEAP mRNA levels. The activity of promoters/enhancers and other elements can be measured due to their direct correlation to SEAP secretion. Finally, the SEAP phosphatase is heat persistent and endures a temperature of 65°C, whereas other phosphatases degrade at this temperature. Therefore, heat treatment can be used to selectively enrich SEAP in samples that might contain additional phosphatases.

<figure id="fig:optogenetic-switch" class="align-left" style="width: 100%; display: block; margin-right: auto">

![Figure 15](/img/user/figures/BLUE_gene_switch.png)

<figcaption>
<strong>Figure 15.</strong> 

</figcaption>
</figure>

> **Mode of function of the optogenetic gene switch in genomically-engineered cells.** **A)** An engineered LOV2 domain from *Avena sativa* phototropin 1 was fused to the C-terminus of the E-protein (erythromycin resistance protein), thus tethering it to a response construct harboring 8 repeats of the E binding sequence (*etr8*) upstream of a synthetic minimal promoter, while the PDZ interaction domain was fused to the VP16 transactivation domain. In the dark, the epitope tag of the LOVpep fusion protein is inaccessible for the PDZ domain. Consequently, gene expression is off. Blue light (460 nm) illumination leads to the unwinding of the C-terminal Jα helix of LOVpep and makes the epitope tag accessible for binding of the PDZ domain. Due to the recruitment of the transactivator VP16 to the minimal promoter, the transcriptional machineries are recruited, and the SEAP gene‑expression is induced. Schematic representation of the vector encoding the photo-switch **(B)** and the SEAP reporter gene **(C)** both flanked by inverted terminal repeats (ITRs).

### Materials

<figure id="tbl:materials-exp2" class="align-left" style="width: 100%; float: left; margin-right: 1em">
  <figcaption>
    <strong>Table 12.</strong> 

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

#### Day 1: Seeding Mammalian Cells 

Preparation of materials:

- Pre-warm Ham’s medium, 1X PBS, and Trypsin/EDTA in 37°C water bath.
- 15 mL falcons, stripette tips (10 mL), 1000 µL and 200 µL tips (sterilized).
- 24-well cell-culture plates for cell seeding.
- Fuchs-Rosenthal counting chamber.

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

**Determine volume of original cell suspension needed:** $$V_{\text{suspension}}\ (\text{mL}) = \frac{C_{\text{target}} \times V_{\text{total}}}{C_{\text{orig}}}$$

**Determine volume of fresh medium needed to reach final volume:** $$V_{\text{medium}}\ (\text{mL}) = V_{\text{total}} - V_{\text{suspension}}$$

**Next Step at the Bench:** Add $V_{\text{suspension}}$ of your cells to a sterile tube containing $V_{\text{medium}}$ of fresh medium. Mix gently, then pipette your standard volume (e.g., $500\ \mu\text{L}$) into each well.

1.  For each group: 4 wells as replicates of each time point (t1 and t2), 2 different incubation conditions (light and dark), therefore prepare 16+1 wells per group and seed into 2 **different** plates!
2.  Prepare the calculated cells suspension (50,000 cells per well) and medium in a 50 mL falcon (master mix).
3.  Add 500 µL to each well.

Incubate the cells overnight at 37°C in the CO~2~ incubator.

#### Day 2: Illumination / t0 and t1 Supernatant Collection 

Preparation of materials:

- Pre-warm Ham’s in a 37°C water bath.
- 15 mL Falcon tubes, stripette tips (10 mL), 1000 µL, and 200 µL tips.
- Light boxes adjusted to blue light 460 nm with a light intensity of 10 μmol m^-2^ s^-1^.
- Round bottom 96-well plate.

Procedure:

1.  Check the cells under the microscope.

For collecting the t0 sample, we will proceed as follows:

- Groups 1-4 will take the supernatant without any medium change.
- Groups 5-8 will perform a medium change before taking the supernatant.

1.  Take 200 µL supernatant from each well into the 96-well plate as “0 h” sample (Groups 1-4).
2.  Remove the rest medium and add 500 µL of fresh medium into each well.
3.  Transfer 200 µL of the freshly exchanged medium from each well into the 96-well plate as “0 h” sample (Groups 5-8). Replace the 200 µL taken.
4.  Transfer one of your 24-well plates into a light box with 10 μmol m^-2^ s^-1^ blue light and the other one into the dark box.
5.  After 6 h illumination, take 200 µL supernatant from the t1 wells of each plate into the 96-well plate (clear, round bottom) in the laminar flow bench under green light. Return the cells to the light boxes in the incubator.
6.  Seal the 96-well plate with tape (make sure it is well sealed).
7.  Store at -20°C.

#### Day 3: t2 Supernatant Collection and SEAP Assay 

Preparation of materials:

- Transparent 96-well plate (flat bottom).
- 2x SEAP buffer and para-nitrophenyl-phosphate (pNPP) substrate.
- PBS.
- Multichannel and multi-stepper pipettes with tips.

1.  After 24 h illumination, transfer 200 µL of cell supernatant from the t2 wells into the 96-well plate.
2.  Incubate the sealed round-bottom 96-well plate for 45 min at 65°C.
3.  Add 100 µL of SEAP buffer into each well of a flat-bottom 96-well plate using the multi-stepper pipette.
4.  Add 80 µL of supernatant from the round-bottom 96-well plate. For samples from timepoint t2, first add 40 µL PBS and then only 40 µL of supernatant.
5.  Set up the program at the plate reader (Absorbance 1h: spectroscopic measurement every minute (60 times, ca. 1 h); wavelength 405 nm.)
6.  Remove air-bubbles with toothpicks.
7.  Add 20 µL of pNPP substrate using the multi-stepper pipette. Be fast, as the reaction starts immediately after adding the substrate to the first well. One person should add the substrate for the entire plate. Place the plate immediately into the plate reader and start the measurement.

<figure id="fig:seap-formula" class="align-left" style="width: 80%; display: block; margin-right: auto">

![Figure 16](/img/user/figures/seap_formula.png)

<figcaption>
<strong>Figure 16.</strong> 
Pipetting scheme.
</figcaption>
</figure>

Hints for data processing:

Subsequent determination of the SEAP activity \[U/L\] is performed by calculating the slope of the  
respective curves \[OD/min\] and the Lambert-Beer law, resulting in the following formula:

∈ = 18,600 M^-1^cm^-1^; d= length of the light path \[cm\] (typically 0.5 cm); = amount of SEAP‑containing supernatant / dilution factor of the sample; = used volume of supernatant.

It is highly recommended to develop a template with Microsoft Excel for data processing.

## Experiment III: Protein Trans-Splicing for Bacterial Logic Gate Design

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

<figure id="fig:logic-gate" class="align-left" style="width: 80%; display: block; margin-right: auto">

![Figure 17](/img/user/figures/inteins_boolean_gates.png)

<figcaption>
<strong>Figure 17.</strong> 
** Scheme for the protein <em>trans</em>-splicing experiment to design
logic gates.
</figcaption>
</figure>

### Materials

<figure id="tbl:materials-exp3" class="align-left" style="width: 100%; float: left; margin-right: 1em">
  <figcaption>
    <strong>Table 13.</strong> 
Materials used in Experiment III.
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
<td>Arabinose</td>
<td>20%</td>
<td>Induce expression of PBAD</td>
</tr>
<tr>
<td>Ampicillin</td>
<td>100 mg/mL</td>
<td>Selection marker</td>
</tr>
<tr>
<td>Kanamycin</td>
<td>50 mg/mL</td>
<td>Selection marker</td>
</tr>
<tr>
<td>IPTG</td>
<td>1 M</td>
<td>Induce expression of PT7</td>
</tr>
<tr>
<td>LB-Medium</td>
<td>10 g/L tryptone, 5g/L yeast extract, 10 g/L NaCl, pH 7.0.</td>
<td>Bacteria growth medium</td>
</tr>
<tr>
<td>PBS</td>
<td>2.7 mM KCl, 1.5 mM KH<sub>2</sub>PO<sub>4</sub>, 8.0 mM
Na<sub>2</sub>HPO<sub>4</sub>, 137 mM NaCl in dH<sub>2</sub>O</td>
<td>Buffer used for cell diluting</td>
</tr>
<tr>
<td><em>E. coli</em> T7 express strain</td>
<td></td>
<td>Expresses T7 RNA- polymerase</td>
</tr>
</tbody>
</table>
</figure>

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

<figure id="tbl:experimental-setup" class="align-left" style="width: 100%; float: left; margin-right: 1em">
  <figcaption>
    <strong>Table 14.</strong> 

  </figcaption>
<table>
<thead>
<tr>
<th>Plasmid</th>
<th>Gr. 1</th>
<th>Gr. 2</th>
<th>Gr. 3</th>
<th>Gr. 4</th>
<th>Gr. 5</th>
<th>Gr. 6</th>
<th>Gr. 7</th>
<th>Gr. 8</th>
</tr>
</thead>
<tbody>
<tr>
<td>pDD259</td>
<td>I</td>
<td>I</td>
<td>-</td>
<td>-</td>
<td>I</td>
<td>I</td>
<td>I</td>
<td>I</td>
</tr>
<tr>
<td>pDD262</td>
<td>I</td>
<td>I</td>
<td>-</td>
<td>-</td>
<td>-</td>
<td>-</td>
<td>-</td>
<td>-</td>
</tr>
<tr>
<td>pDD260/261</td>
<td>I/A</td>
<td>I/A</td>
<td>I/A</td>
<td>I/A</td>
<td>I/A</td>
<td>I/A</td>
<td>I/A</td>
<td>I/A</td>
</tr>
<tr>
<td>pDD260/261 (alt)</td>
<td>-</td>
<td>-</td>
<td>-</td>
<td>-</td>
<td>I</td>
<td>I</td>
<td>A</td>
<td>A</td>
</tr>
</tbody>
</table>
</figure>

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

## Experiment IV: Intein-Catalyzed Protein Domain Swapping at the Plasma Membrane

**Supervisors:** Cha San Koh, Daniel Wiebensohn, Hannes Beyer

koh@hhu.de, dawie106@hhu.de, hannes.beyer@huu.de

This experiment aims to induce either the addition or exchange of two protein domains at the plasma membrane of mammalian HeLa cells using split intein technology. Here, the construct design determines whether an intein *trans*-splicing reaction yields one of the two possible outcomes. To determine the localization of the two proteins, we will use the green fluorescent protein GFP and the red fluorescent protein mCherry, allowing for their analysis via confocal fluorescence microscopy (**Figure 18**). Both fluorescent proteins are genetically fused to one half of the DnaE intein from *Nostoc punctiforme* (*Npu*DnaE intein split fragments, abbreviated as IntN and IntC for the N- and C-terminal fragment, respectively), which you also used in Experiment III. GFP is additionally fused to an N-terminal myristylation/palmitylation signal derived from the Src kinase Lck, leading to cotranslational myristoylation at glycine residue 2 and then posttranslational palmitoylation at cysteine residues 3 and 5 (Akimzhanov and Boehning, 2015). Modification with these fatty acids leads to the attachment of the protein to inner cell membranes.

In the experiment, you will transiently transfect human HeLa cells with different combinations of the following plasmids encoding two versions of the membrane-attached GFP protein fused to IntN, or cytosolic mCherry fused to IntC. While we expect GFP to localize at the membrane and mCherry in the cytosol when transfected into cells, their cotransfection should induce the protein splicing reaction, which we will observe by confocal microscopy.

<figure id="fig:domain-swapping" class="align-left" style="width: 100%; display: block; margin-right: auto">

![Figure 18](/img/user/figures/inteins_plasms_membrane.png)

<figcaption>
<strong>Figure 18.</strong> 
** Split intein-catalyzed protein trans-splicing (PTS) reaction either
leading to the addition (left), or exchange (right) of GFP and mCherry
at the plasma membrane, depending on the domain order of the GFP
constructs (pDD130 vs pDD132). The IntC-fused mCherry construct pDD131
is identical in both approaches.
</figcaption>
</figure>

In cells, many relevant signaling pathways initiate or pass through microdomains at the plasma membrane, often linking the perception of extracellular signals via membrane integral receptors to the cytosol. Therefore, modulating the localization of proteins involved in cell signaling represents an important tool to regulate cellular behavior. However, the induction of protein domain swapping might likewise be employed to regulate diverse cellular mechanisms, for example, by exchanging antagonistically functional protein domains, such as activators and repressors.

### Materials

**Plasmids (Minipreps)**

<figure id="tbl:materials-exp4" class="align-left" style="width: 80%; float: left; margin-right: 1em">
  <figcaption>
    <strong>Table 15.</strong> 

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
<td>PSV40-LckM/P-GFP-Int<sub>N</sub>-pA</td>
<td>100 ng/µL</td>
</tr>
<tr>
<td>pDD131</td>
<td>PSV40-Int<sub>C</sub>-mCherry-pA</td>
<td>100 ng/µL</td>
</tr>
<tr>
<td>pDD132</td>
<td>PSV40-LckM/P-Int<sub>N</sub>-GFP-pA</td>
<td>100 ng/µL</td>
</tr>
</tbody>
</table>
</figure>

**Media**

| Name                 | Description/Composition                                                                                                                   |
|----------------------|-------------------------------------------------------------------------------------------------------------------------------------------|
| DMEMcomplete         | Dulbecco’s Modified Eagle Medium (Gibco), 10% fetal bovine serum (FBS, PAN-Biotech), 100 U/mL penicillin, 0.1 mg/mL streptomycin (Gibco). |
| Opti-MEMTM           | Optimized minimum essential medium (Gibco), serum-free.                                                                                   |
| Lysogeny broth (LB)  | 10 g/L tryptone, 5g/L yeast extract, 10 g/L NaCl, pH 7.0.                                                                                 |
| LB-agar plates (Amp) | 20 g/L Bacto Agar in 500 mL dH~2~O, 100 µg/mL Ampicillin.                                                                                 |

**Cells**

| Name            | Description                                                                                                                                                                    |
|-----------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| HeLa            | *H. sapiens* cervix carcinoma derivative, epithelial-like, (ACC 57, DSMZ).                                                                                                     |
| *E. coli* TOP10 | Chemically-competent cells. Genotyp: F-*mcrA* Δ(*mrr-hsd\_RMS-*mcr\_BC) Φ80*Lac*ZΔM15 Δ*Lac*X74 *rec*A1 *ara*D139 Δ(*araleu*) 7697 *gal*U *gal*K *rps*L (StrR) *end*A1 *nup*G. |

**Buffers and chemicals**

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

**Consumables**

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

Please refer to Experiment I <span class="mark">(day 2, p. 22)</span> for the transformation protocol. Use 1 µL of the provided plasmid DNA per transformation into one tube of competent *E. coli* TOP10 cells. Spread 50 µL of culture on one LB-Amp plate (asymmetrically, you want to be able to pick a single colony the next day). Incubate the plate overnight at 37°C.

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

1.  Per well, dilute 0.75 µg of DNA in OptiMEM to a final volume of 50 µL (remember your Midi-prep concentration). Please check **Table 16** and **Table 17** for further information.
2.  When transfecting multiple plasmids for the same setup, divide the total DNA amount (0.75 µg) by the number of plasmids which are transfected (equal plasmid load). Note: keep ca. 0.75 µg as total DNA amount; the ratio of DNA: PEI is important for the transfection efficiency!
3.  Per well, dilute 2.5 µL of PEI solution in OptiMEM to a final volume of 50 µL. Vortex. Please check **Table 16** and **Table 17** for further information.
4.  Add an equal volume of PEI solution to the DNA solution.
5.  Vortex the solution immediately and thoroughly for 10 s. Complexation of PEI with DNA, into small particles able to enter the cell during transfection, is dependent on thorough mixing at this step.
6.  Incubate for 15 min at RT.
7.  Per well, add the premixed 100 µL PEI/DNA mix drop-wise to each well. DO NOT VORTEX!
8.  Incubate for 4 h at 37°C in the cell culture incubator.
9.  Exchange medium for fresh cultivation medium (500 µL per well).

<figure id="tbl:transfection-odd" class="align-left" style="width: 100%; float: left; margin-right: 1em">
  <figcaption>
    <strong>Table 16.</strong> 
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
    <strong>Table 17.</strong> 
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

## Experiment V: Engineering Chemically Regulated Gene Switch Technology in Stable Mammalian Cell Culture

**Supervisors:** Maria Evangelopoulou, Miriam Labusch, Benjamin McLean

maria.evangelopoulou@hhu.de, benjamin.mclean@hhu.de, miriam.labusch@hhu.de

### Aim

The aim of this experiment is to investigate the dose-dependent induction of neonGreen expression using the tetracycline-inducible system and quantify fluorescence levels via flow cytometry. Each group will generate stable transgenic CHO-K1 lines carrying both the reporter and tetR, and will then measure fluorescence in a control sample without tetracycline, as well as in one experimental sample containing a given tetracycline concentration to compare expression levels.

### Background

#### Tetracycline-Inducible Expression System (Tet System)

The tetracycline (Tet) system is a widely used inducible gene expression system that enables precise control over the transcription of a gene of interest. It is based on regulatory elements derived from the *Escherichia coli* tetracycline resistance operon. The system typically consists of two components:

1.  A **t**etracycline-controlled **t**rans**a**ctivator (tTA or rtTA-reverse rTA), which binds to tetracycline response elements (TRE) upstream of the gene of interest.
2.  The target gene, in this case coding for the fluorescent protein neonGreen, downstream of the TRE.

<figure id="fig:tet-system" class="align-left" style="width: 70%; display: block; margin-right: auto">

![Figure 19](/img/user/figures/Tet-On.png)

<figcaption>
<strong>Figure 19.</strong> 
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
    <strong>Table 18.</strong> 

  </figcaption>
<table>
<colgroup>
<col style="width: 20%" />
<col style="width: 50%" />
<col style="width: 30%" />
</colgroup>
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

**Plasmids (Midipreps)** &gt; \[!table\] \#tbl:yourtablelabel width=100% align=center columns=0.25,0.45,0.30 colsep=4pt fontsize=footnotesize spacing=1.1 &gt; &gt; Used plasmids prepared by the supervisors.

| Name   | Description                                 | Concentration |
|--------|---------------------------------------------|---------------|
| pDD312 | PCAG-TetOn3G-Tbg - Ptre3gv-mneonGreen-TSV40 | 1926 ng/µL    |
| pME001 | PT7-PB transposase- TSV40                   | 2126 ng/µL    |

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

**Determine volume of original cell suspension needed:** $$V_{\text{suspension}}\ (\text{mL}) = \frac{C_{\text{target}} \times V_{\text{total}}}{C_{\text{orig}}}$$

**Determine volume of fresh medium needed to reach final volume:** $$V_{\text{medium}}\ (\text{mL}) = V_{\text{total}} - V_{\text{suspension}}$$

**Next Step at the Bench:** Add $V_{\text{suspension}}$ of your cells to a sterile tube containing $V_{\text{medium}}$ of fresh medium. Mix gently, then pipette your standard volume (e.g., $500\ \mu\text{L}$) into each well.

#### Day 3 - Stable Transfection

For this part of the experiment three groups will form one big group to transfect one well per group, so in the end we would have three transfected wells. These groups will then share the responsibility of passaging and selecting the cells until the day of seeding for the experiment.

**What you will need**

- Pre-warmed OptiMEM (37°C water bath)
- Polyethyleneimine (PEI)
- 1.5 mL tubes, 10 µL, 200 µL and 1000 µL sterile tips
- Cells seeded in 6-well plate
- Plasmids: pME001 (piggybac transposase), pDD312 (tet inducible neonGreen expression)

<figure id="tbl:yourtablelabel" class="align-center" style="width: 100%; display: block; margin-left: auto; margin-right: auto">
  <figcaption>
    <strong>Table 19.</strong> 
<strong>This is the table caption…</strong>
  </figcaption>
<table>
<colgroup>
<col style="width: 25%" />
<col style="width: 45%" />
<col style="width: 30%" />
</colgroup>
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
7.  Medium exchange \~ 4h after transfection.
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

# References

Akimzhanov, A.M., and Boehning, D. (2015). Rapid and transient palmitoylation of the tyrosine kinase Lck mediates Fas signaling. Proc. Natl. Acad. Sci. U. S. A. 112, 11876–11880.

Beyer, H.M., Gonschorek, P., Samodelov, S.L., Meier, M., Weber, W., and Zurbriggen, M.D. (2015). AQUA Cloning: A Versatile and Simple Enzyme-Free Cloning Approach. PLOS ONE 10, e0137652.

Friedel, K., Popp, M.A., Matern, J.C.J., Gazdag, E.M., Thiel, I.V., Volkmann, G., Blankenfeldt, W., and Mootz, H.D. (2019). A functional interplay between intein and extein sequences in protein splicing compensates for the essential block B histidine. Chem. Sci. 10, 239–251.

Mátés, L., Chuah, M.K.L., Belay, E., Jerchow, B., Manoj, N., Acosta-Sanchez, A., Grzela, D.P., Schmitt, A., Becker, K., Matrai, J., et al. (2009). Molecular evolution of a novel hyperactive Sleeping Beauty transposase enables robust stable gene transfer in vertebrates. Nat. Genet. 41, 753–761.

Müller, K., Naumann, S., Weber, W., and Zurbriggen, M.D. (2015). Optogenetics for gene expression in mammalian cells. Biol. Chem. 396, 145–152.
