---
{"dg-publish":true,"permalink":"/garden-02-background/","title":"Background"}
---


# Background

## Protein Switches

Proteins constitute a group of macro-biomolecules that provide cells with unique functions essential for life. Comprising one or several chains of amino acids, proteins adopt complex 3-dimensional shapes serving as scaffolds for their biological role. Within organisms, proteins act, for example, as biocatalysts involved in cell metabolism or homeostasis (e.g., replication of the genome, energy conversion, protein synthesis, signal propagation). Proteins further provide structure to cells and organisms, engage in intra- and extracellular communication (cell signaling cascades, hormones, receptors and ligands, transporters, etc.), or regulate each other (feedback loops, induction of events such as transcription, translation, polymerization, mobility, etc.). Due to the wide range of different biological functions inherent to natural proteins, they offer unique opportunities for engineering novel protein-based functions, for example, using synthetic biology-inspired approaches.

### Engineered Protein Switches and Optogenetics

Inducible gene expression switches are an example of engineered protein switches. Chemically controlled molecular switches have played a central role in the fundamental study of life, and the emergence of synthetic biology. They have become routine tools in cell biology research and industry (**[Figure 3](#fig:tetracycline-switch)**).

<figure id="fig:tetracycline-switch" class="float-right" style="width: 45%; float: right; margin-left: 1em">

![Figure 3](/img/user/figures/tetracycline.png)
<figcaption style="font-size: 0.9em; color: #555; margin-top: 0.5em; line-height: 1.5; font-style: normal; display: block;">

<strong style="color: #333;">Figure 3.</strong> Tetracycline-inducible gene expression switch based on an engineered protein switch, the reversed tetracycline transactivator (rtTA). The engineered “reversed” bacterial repressor protein rTetR binds to a cognate operator DNA sequence (Tet-response element, TRE) in the presence of the antibiotic tetracycline. rTetR is fused to a viral transactivator VP16 which induces gene expression from a minimal promoter (Pmin) upon DNA binding to induce transcription of a gene of interest (goi).

</figcaption>

</figure>

> *Note: the natural bacterial tetracycline repressor protein TetR acts as a repressor of transcription in gram-negative bacteria and releases DNA in the presence of tetracycline to induce the expression of resistance genes (TetR, the repressor; and TetA, the protein that pumps antibiotic tetracycline extracellularly).*

However, drawbacks inherent to small molecules like tetracycline, such as difficulties in removing the inducer and diffusion-based transport, have prevented rapid reversibility and spatially-resolved activation. In contrast, light offers unprecedented spatial and temporal resolution. Consequently, the development of light-controlled devices is highly desirable and has recently received much attention, resulting in a variety of different light-controlled tools in bacteria and yeast as well as in mammalian cells. These control diverse cellular activities, including gene expression.

The first light-controlled molecular tools were constructed by introducing photo-cleavable inhibiting chemical groups into inducers, nucleic acids, and transactivators that could be cleaved off in response to UVB light. However, a significant disadvantage of this method is the need to exogenously apply the caged molecules or to reprogram the translation machinery for the incorporation of non-natural amino acids. This disadvantage has been overcome by the optogenetic approach that combines optical and genetic methods to develop light-responsive tools. The first breakthrough in mammalian optogenetics was the discovery of microbial opsins and their subsequent introduction in neuroscience, which revolutionized the study of neuronal networks. Channelrhodopsin, the first opsin that was applied in mammalian neurons, becomes permeable to cations upon blue light illumination, thus triggering neuronal activation. Later, channelrhodopsin was complemented by other ionotropic receptors, including the orange light-responsive, chloride pump halorhodopsin, which made it possible to use dual‑wavelength control to excite or inhibit neurons with subcellular resolution, even in intact brain tissue and in moving animals. Moving beyond neuroscience, more recent optogenetic tools have been engineered to control diverse signaling processes on the protein level in mammalian cells, including gene expression and protein stability, subcellular localization of proteins, receptor and kinase activity, organelle movement, etc. To this end, photoreceptors from all kingdoms of life that naturally sense environmental light information by responding to light of distinct regions of the light spectrum have been employed as engineering scaffolds based on modulating protein-protein interactions, or protein conformation in response to light stimulation (Müller et al., 2015). **[Figure 4](#fig:photoswitchable-domains)** illustrates two photoreceptors that are frequently employed in optogenetic protein engineering approaches.

<figure id="fig:photoswitchable-domains" class="align-left" style="width: 100%; display: block; margin-right: auto">

![Figure 4](/img/user/figures/photoswitches.png)
<figcaption style="font-size: 0.9em; color: #555; margin-top: 0.5em; line-height: 1.5; font-style: normal; display: block;">

<strong style="color: #333;">Figure 4.</strong> <strong>Photoswitchable domains frequently used for optogenetic engineering. A)</strong> <em>A. thaliana</em> Phytochrome B (PhyB) photoreceptor. Red light (R) induces a conformational change in PhyB via a bound linear billin chromophore (not shown), allowing it to heterodimerize with Phytochrome-Interacting-Factor 6 (PIF6). Far-red light (FR) induces the dissociation of the PhyB/PIF6 complex. <strong>B)</strong> Light-Oxygen-Voltage LOV2 domain of <em>Avena sativa</em> phototropin 1 uses a flavin mononucleotide (FMN, not illustrated) to sense blue light. Photoexcitation leads to relaxation of helix Jα, which rewinds in darkness. <em>As</em>LOV2 is often used either to cage peptides in the dark state (top), or when inserted into other proteins, to induce structural remodeling upon light treatment which influences the function of the target protein.

</figcaption>

</figure>

### Protein Splicing

Protein splicing is a natural phenomenon catalyzed by autocatalytic protein domains called inteins (internal proteins). Inteins reside within other proteins, usually close to the active site of proteins, which are essential for the fitness of a given organism. After translation, inteins autocatalytically excise themselves from the precursor protein and covalently ligate the flanking protein sequences (exteins) with a regular peptide bond, a process called protein *cis*-splicing, thereby functionally reconstituting the sequence of the host proteins (**[Figure 5A](#fig:protein-splicing)**).

<figure id="fig:protein-splicing" class="align-left" style="width: 100%; display: block; margin-right: auto">

![Figure 5](/img/user/figures/inteins.png)
<figcaption style="font-size: 0.9em; color: #555; margin-top: 0.5em; line-height: 1.5; font-style: normal; display: block;">

<strong style="color: #333;">Figure 5.</strong> <strong>Protein splicing in <em>cis</em> and <em>trans</em>. A)</strong> After protein synthesis, protein cis-splicing leads to the self-catalyzed excision of an intein from a precursor protein and the covalent ligation of the flanking extein sequences. <strong>B)</strong> In protein trans-splicing, the association of split intein fragments (IntN and IntC) initiates reconstitution of the intein and triggers protein splicing in trans, leading to the ligation of individual polypeptides.

</figcaption>

</figure>

Little is known about the biological relevance of inteins and therefore, they are mainly seen as selfish genetic elements capable of inserting into protein-encoding genes. Because inteins tend to insert into genes encoding essential proteins with a high degree of conservation, they may be maintained within populations as long as they sufficiently catalyze their self-removal, thereby escaping genetic drifts. However, it seems plausible that some inteins might act as environmental sensors and regulate the activity of their host proteins accordingly (e.g., reduce the growth rate under stress conditions). From genome-mining approaches, split inteins have been identified which can ligate individual polypeptides upon fragment complementation of a N- and C-intein fragment (Int<sub>N</sub> and Int<sub>C</sub>) in a protein trans-splicing reaction (**[Figure 5B](#fig:protein-splicing)**). Additionally, one can often engineer *cis*-splicing into *trans*-splicing inteins. Protein *cis*-splicing gave rise to a variety of applications as it allows covalently ligating protein sequences in a solvent-free medium (*in vivo* or *in vitro*) without the requirement of additional cofactors and energy sources. Protein splicing of class 1 inteins, representing the most frequently-found examples, occurs in 4 concerted steps, involving the first intein residue (Cys 1 or Ser 1), the first residue of the C‑terminal extein (Cys/Ser/Thr +1), and the last intein residue (typically Asn) (**[Figure 4](#fig:photoswitchable-domains)**).

<figure id="fig:splicing-mechanism" class="align-left" style="width: 70%; display: block; margin-right: auto">

![Figure 6](/img/user/figures/intein_mechanism.png)
<figcaption style="font-size: 0.9em; color: #555; margin-top: 0.5em; line-height: 1.5; font-style: normal; display: block;">

<strong style="color: #333;">Figure 6.</strong> <strong>Conventional protein splicing mechanism of class 1 inteins.</strong> Step 1: N-S acyl shift of the Cys 1 (in some cases Ser 1) and the N-terminal extein to form a linear thioester. Step 2: Trans-esterification of Cys +1 (in some cases Ser/Thr +1) to a branched intermediate where the N- and C-exteins are already covalently connected and the intein is still attached. Step 3: Asn cyclization into a succinimide, thereby releasing the intein. Step 4: Spontaneous O-N shift rearrangement into the energetically-favorable peptide bond (not intein-catalyzed). Figure modified from Friedel <em>et al.</em>, 2019.

</figcaption>

</figure>

Split inteins in particular found a wide range of applications including their use for protein labeling, protein semi-synthesis, protein purification, protein cyclization, or for engineering protein logic gates. **[Figure 7](#fig:split-intein-apps)** summarizes some recent examples of developments utilizing split intein technologies (Friedel *et al*., 2019).

<figure id="fig:split-intein-apps" class="align-left" style="width: 100%; display: block; margin-right: auto">

![Figure 7](/img/user/figures/inteins_applications.png)
<figcaption style="font-size: 0.9em; color: #555; margin-top: 0.5em; line-height: 1.5; font-style: normal; display: block;">

<strong style="color: #333;">Figure 7.</strong> <strong>Applications of split intein technologies.</strong> Bi-specific antibodies ligated in vitro using split inteins and individual Fab fragments. <strong>Biosensors</strong> to detect caspases. <em>In vivo</em> cyclization of the fluorescent protein mNeonGreen2 abolishes fluorescence. Cleavage of the engineered DEVD sequence by caspases releases the cyclic tension, resulting in fluorescence. <strong>Gene therapy</strong> facilitated by individual packaging of two split CRISPR Cas9 enzyme fragments into adeno associated viral vectors (AAVs), thereby respecting the viral packaging capacity. Intein trans splicing reconstitutes the Cas9 enzyme upon co-infection of a target cell with both vectors.

</figcaption>

</figure>

## AQUA Cloning

The implementation of synthetic biology approaches, for example to the study of cell signaling, demands a wide variety of constructs, including complex combinations of synthetic protein modules, promoters, reporters, etc. The cloning of numerous constructs is time and cost demanding, therefore novel cloning approaches are necessary to simplify the engineering process. One of such methods is AQUA Cloning (**[Figure 8](#fig:aqua-cloning)**). During the practical part you will be introduced into this technique: Multiple DNA fragments sharing 20-60 bp overlap can easily be assembled into vectors in *E. coli* cells, based on *in vivo* recombination, omitting the need for enzymes commonly mediating the DNA cloning reaction in a test tube. In the practical course you will use a polymerase chain reaction (PCR) and AQUA Cloning as well as conventional restriction and ligation cloning to construct bacterial vectors encoding a split intein-based protein logic gate for an experiment in the following week. At the same time, you will engineer suitable control vectors. The resulting vectors will be analyzed using analytical restriction enzyme digestion and agarose gel electrophoresis, followed by Sanger sequencing.

<figure id="fig:aqua-cloning" class="align-left" style="width: 100%; display: block; margin-right: auto">

![Figure 8](/img/user/figures/aqua_workflow.png)
<figcaption style="font-size: 0.9em; color: #555; margin-top: 0.5em; line-height: 1.5; font-style: normal; display: block;">

<strong style="color: #333;">Figure 8.</strong> <strong>AQUA Cloning.</strong> Advanced quick assembly cloning is a simple yet versatile cloning method (Beyer et al., 2015). (<strong>a</strong>) DNA parts are produced by PCR, or restriction digest (or both). Oligonucleotides are designed to contribute flanking homologous regions to adjacent DNA fragments of optimally 32 bp in length. DNA parts are assembled into a circular plasmid by sequence-determined directionality <em>in vivo</em> by <em>E. coli</em>. (<strong>b</strong>) AQUA Cloning work-flow. (1) DNA parts are generated by PCR amplification, or derive from an enzymatic digestion. (2) Next, DNA parts are purified by gel-electrophoresis and (3) mixed and simply incubated in water prior to transformation into chemically competent <em>E. coli</em> Top10 cells for <em>in vivo</em> assembly. (4) Finally, the obtained colonies are confirmed for correct assembly by standard methods such as analytical PCR, restriction digest, and/or comprehensive sequencing.

</figcaption>

</figure>

## Transfection of Mammalian Cells

The process of introducing nucleic acids into mammalian cells by non-viral methods is defined as transfection. By using various chemicals, lipid-based or physical methods, this gene transfer technology is a powerful tool to study gene function and protein expression in the context of a cell. Basically, transfection is a method that overcomes the challenge of introducing molecules with a negative charge (e.g. the phosphate backbone of DNA) into cells with a negatively charged membrane.

Ions like calcium or cationic lipid-based reagents coat the DNA, thus creating an overall positive charge that facilitates uptake of the DNA-transfection reagent complex across the cell membrane (**[Figure 9](#fig:transfection-mechanism)**).

<figure id="fig:transfection-mechanism" class="align-left" style="width: 100%; display: block; margin-right: auto">

![Figure 9](/img/user/figures/transfection.png)
<figcaption style="font-size: 0.9em; color: #555; margin-top: 0.5em; line-height: 1.5; font-style: normal; display: block;">

<strong style="color: #333;">Figure 9.</strong> <strong>Transfection using chemical reagents. A)</strong> Common cationic transfection reagents for the generation of reagent: DNA complexes with a net positive charge. <strong>B)</strong> Overview of the transfection mechanism. DNA is complexed with the cationic reagent. The positively charged complexes associate to the negatively charged membrane and are taken up by endocytosis. Upon escape from the endosome, the DNA is free to enter the nucleus (e.g., during cell division). Figure created with BioRender.com

</figcaption>

</figure>

In the practical course polyethylenimine (PEI) will be employed to exemplify transfection using chemical reagents.

PEI is a poly-cationic polymer that is mixed with the DNA in a ratio that ensures the formation of complexes that carry a net positive charge. These cationic complexes interact with the negatively charged cell-surface and are taken up by endocytosis. Inside the endosome, PEI acts as a proton sponge, preventing acidification that is required for the activity of endosomal nucleases (**[Figure 10](#fig:pei-transfection)**).

<figure id="fig:pei-transfection" class="align-left" style="width: 100%; display: block; margin-right: auto">

![Figure 10](/img/user/figures/transfection_pei.png)
<figcaption style="font-size: 0.9em; color: #555; margin-top: 0.5em; line-height: 1.5; font-style: normal; display: block;">

<strong style="color: #333;">Figure 10.</strong> <strong>Polyethyleneimine (PEI)-mediated transfection of mammalian cells. (a)</strong> Chemical structure <strong>(b)</strong> Mechanism of PEI-mediated transfection. The positively charged PEI:DNA complexes are taken up by endocytosis. Inside the endosome PEI prevents acidification, which eventually leads to rupture of the endosome and liberation of the DNA into the cytoplasm.

</figcaption>

</figure>

## Genome Engineering of Mammalian Cells

Upon transfection into mammalian cells, nucleic acids can contribute to the genetic programming and instruct cells to execute or alter particular activities. Commonly, either RNA- or DNA-molecules are employed, which in most cases perform their biological function in the cytoplasm and nucleus, respectively. Current RNA-based Covid-19 vaccines, for example, rely on mRNA which upon cell uptake, undergoes ribosomal translation into fragments of the viral spike protein in the cytosol. For the production of biopharmaceuticals and research purposes in cell lines, DNA plasmids are commonly used, which require nuclear entry in order to reach the cell compartment where RNA transcription takes place (**[Figure 11](#fig:mammalian-plasmid)**).

<figure id="fig:mammalian-plasmid" class="align-left" style="width: 70%; display: block; margin-right: auto">

![Figure 11](/img/user/figures/mammalian_cell_plasmid.png)
<figcaption style="font-size: 0.9em; color: #555; margin-top: 0.5em; line-height: 1.5; font-style: normal; display: block;">

<strong style="color: #333;">Figure 11.</strong> Example of a mammalian cell plasmid including mammalian cell-specific, as well as bacterial features.

</figcaption>

</figure>

Both examples lead to a transient activity of the transfected genetic material. However, over time, the RNA/DNA will be cleared, usually within a time frame of a few days. In rare cases, transfected DNA can integrate at random positions into the cell genome (roughly in 1 out of 1.000 transfected cells, strongly depending on the cell, construct, and the exact experimental conditions). By using additional eukaryotic antibiotic resistance genes encoded on the transfected plasmid, one can positively select for these cells. During the past years, several methods have been developed that facilitate the targeted integration of genetic material into mammalian cells or the specific alteration of the cellular genomes. During the theoretical parts of the course, you will have the possibility to familiarize yourself with some examples spanning this topic. Methods to integrate genetic information into cell genomes for example rely on (i) the above-mentioned random DNA integration, (ii) viral gene vehicles, e.g. using lentiviral systems harboring reverse transcriptases and integrases, (iii) homologous recombination-based techniques including the use of recombinases or designer endonucleases and homology templates containing the desired genetic information, or (iv) transposase-technologies originating from transposons (“jumping genes”) which excise and integrate genetic information. Table **[Table 1](#tbl:integration-methods)** summarizes particular properties of these four groups.

Experiment II of this practical course will introduce you to a blue light-sensitive optogenetic gene expression system. Here, you will use mammalian cells that have genomic integrations for the required optogenetic switches and the target gene, which will be expressed upon stimulation with light. These cells were generated using the Sleeping Beauty SB100X transposase, as explained in **[Figure 12](#fig:sleeping-beauty)**. “Sleeping Beauty” refers to a transposase that was originally identified as an inactive enzyme in salmonid fish. Targeted mutagenesis, however, restored the activity after a long evolutionary sleep, and rounds of directed evolution finally yielded a hyperactive transposase enzyme, which is nowadays widely used for genome engineering purposes (Mátés et al., 2009).

<figure id="fig:sleeping-beauty" class="align-left" style="width: 80%; display: block; margin-right: auto">

![Figure 12](/img/user/figures/transposases.png)
<figcaption style="font-size: 0.9em; color: #555; margin-top: 0.5em; line-height: 1.5; font-style: normal; display: block;">

<strong style="color: #333;">Figure 12.</strong> <strong>Mode of function of SB100X Sleeping Beauty-catalyzed transposition.</strong> Cotransfection of plasmids (i) containing a genetic cargo which is flanked by inverted terminal repeats (ITRs), and (ii) a transiently-expressed SB100X transposase gene leads to transposition of the cargo into the cell genome. SB100X excises the genetic cargo from the plasmid and integrates it at random positions (TA sites) into the host genome. Abbreviations: GOI, gene of interest; P, promoter; Res, resistance gene.

</figcaption>

</figure>

<figure id="tbl:integration-methods" class="align-left" style="width: 100%; float: left; margin-right: 1em">
  <figcaption style="font-size: 0.9em; color: #555; margin-bottom: 0.5em; line-height: 1.5; font-style: normal; display: block;">
    <strong style="color: #333;">Table 1.</strong> Properties of the discussed genomic integration method groups.
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
  <figcaption style="font-size: 0.9em; color: #555; margin-bottom: 0.5em; line-height: 1.5; font-style: normal; display: block;">
    <strong style="color: #333;">Table 2.</strong> Mammalian cell-lines (Descriptions from Deutsche Sammlung von Mikroorganismen und Zellkultur GmbH (DSMZ) and the American type culture collection (ATCC)).
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

----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

[← Previous](garden_01-Course-Information.md) \| [Next →](garden_03-Experiment1.md)
