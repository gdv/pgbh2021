---
title: Why pangenomics?
date: {{ .Date }}
draft: true
---

The Human Genome Project's assembly of the first genome took 13 years and cost $2.7 billion\cite. Today, consumers can sequence their whole genomes for as little as $300.
Yet most biomedical researchers continue to use a single linear reference genome to assemble larger genome sequences, detect gene variation, and determine gene function.

Who defines this reference genome?

How is it possible to capture the entire diversity of a species with an arbitrary single linear sequence?

In contrast, a *pangenome* is a collection of genomes organized into a graph data
structure to be used for holistic genetic analysis.
It is hard to overstate the impact of moving from a sequence-based to a graph-based view of genetics.
A traditional single sequence-based reference genome might be missing up to 10% of the genetic sequence in under-represented populations~\cite{Sherman:2020}; these missing sequences are the unexplored `dark matter` of the genetic universe.
Today, all human DNA variants are identified comparing with this `standard` reference genome. Even though the `standard' reference was a massive step forward at the time, it is now known to be biased and misrepresents whole populations: for example, 10\% of African DNA sequence does not align to the current reference genome\cite{Sherman:2020}.

For other populations the gap may be smaller but the reference approach is biased and therefore impacts genetical studies of underrepresented populations\cite{Takayama:2021} and even supposedly well represented populations\cite{Ameur:2018}.

This unexplored genomics `dark matter' might include beneficial or harmful traits that traditional techniques are not equipped to study. For example, recent work suggests that a pangenomic approach could have more efficiently discovered a critical genetic variant in the Icelandic population reducing the risk of heart attacks and a different critical variant increasing the risk of dementia~\cite{Sherman:2020}.

Pangenomics will transform the software stack in computational biology, requiring new graph data structures and new algorithms for graph construction, alignment, annotation, and visualization~\cite{
cpgc-computational-pangenomics-bib2019}.

```
--> Insert image
```

We expect pangenome tools to replace reference-based approaches used in most genomic workflows
today~\cite{Sherman:2020,Eizenga:2020,Sherman:2019}.
As an example of this work and the potential impact of computational pangenomics, consider the pangenome graph for chromosome 20 very recently constructed by our team for the HPRC (Fig.~\ref{HPRC}h). Computational pangenomics revealed a `hairball' in the graph that indicates an unexpected amount of variation in the previously-inaccessible centromeric region.

## Further reading:

```
@article{Eizenga:2020,
  keywords     = {},
  pmid         = {32453966},
  IDS          = {pangenome},
  author       = {Eizenga, J. M. and Novak, A. M. and Sibbesen, J. A. and Heumos, S. and Ghaffaari, A. and Hickey, G. and Chang, X. and Seaman, J. D. and Rounthwaite, R. and Ebler, J. and Rautiainen, M. and Garg, S. and Paten, B. and Marschall, T. and Siren, J. and Garrison, E.},
  title        = {{Pangenome Graphs}},
  journal      = {Annual Review of Genomics and Human Genetics},
  year         = {2020},
  month=AUG,
  volume       = {21},
  pages        = {139-162},
  doi          = {10.1146/annurev-genom-120219-080406},
  url          = {http://www.ncbi.nlm.nih.gov/pubmed/32453966},
  abstract     = {Low-cost whole-genome assembly has enabled the collection of haplotype-resolved pangenomes for numerous organisms. In turn, this technological change is encouraging the development of methods that can precisely address the sequence and variation described in large collections of related genomes. The
se approaches often use graphical models of the pangenome to support algorithms for sequence alignment, visualization, functional genomics, and association studies. The additional information provided to these methods by the pangenome allows them to achieve superior performance on a variety of bioinformatic tasks, in
cluding read alignment, variant calling, and genotyping. Pangenome graphs stand to become a ubiquitous tool in genomics. Although it is unclear whether they will replace linearreference genomes, their ability to harmoniously relate multiple sequence and coordinate systems will make them useful irrespective of which p
angenomic models become most common in the future.},
}


@article{Sherman:2020,
  keywords     = {},
  pmid         = {32034321},
  author       = {Sherman, R. M. and Salzberg, S. L.},
  title        = {{Pan-Genomics in the Human Genome Era}},
  journal      = {Nature Reviews Genetics},
  year         = {2020},
  month=APR,
  volume       = {21},
  number       = {4},
  pages        = {243-254},
  doi          = {10.1038/s41576-020-0210-7},
  url          = {http://www.ncbi.nlm.nih.gov/pubmed/32034321},
  abstract     = {Since the early days of the genome era, the scientific community has relied on a single 'reference' genome for each species, which is used as the basis for a wide range of genetic analyses, including studies of variation within and across species. As sequencing costs have dropped, thousands of new g
enomes have been sequenced, and scientists have come to realize that a single reference genome is inadequate for many purposes. By sampling a diverse set of individuals, one can begin to assemble a pan-genome: a collection of all the DNA sequences that occur in a species. Here we review efforts to create pan-genomes
for a range of species, from bacteria to humans, and we further consider the computational methods that have been proposed in order to capture, interpret and compare pan-genome data. As scientists continue to survey and catalogue the genomic variation across human populations and begin to assemble a human pan-genome,
 these efforts will increase our power to connect variation to human diversity, disease and beyond.}
}
```
