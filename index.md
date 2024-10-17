---
title       : "Phylogeny 2"
subtitle    : "BNS-2002: Genes, Development, and Evolution"
author      : Dr Axel Barlow
job         : "email: a.barlow@bangor.ac.uk"
framework   : io2012        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : zenburn      # {zenburn, tomorrow, solarized-dark, ...}
widgets     : []            # {mathjax, quiz, bootstrap}
mode        : selfcontained # {selfcontained, standalone, draft}
knit        : slidify::knit2slides
logo        : LA_Full_colour_reversed.svg
biglogo     : A1_FullColour.svg
assets      : {assets: ../../assets}
license     : by-nc-sa

---



<!-- adding bold and italic options -->
<style>
em {
  font-style: italic
}
strong {
  font-weight: bold;
}
</style>

## Molecular Ecology and Evolution at Bangor (MEEB)

- 3rd year module "Molecular ecology and evolution"
- https://www.bangor.ac.uk/meeb

<img src="./assets/img/meeb_logo_NEW_no_text.jpg" width="100%" style="display: block; margin: auto;" />

---

## Axel Barlow research group

- Population genomics, Paleogenomics, Conservation genomics
- Dissertation and MSc projects

<img src="./assets/img/extinct_animals.png" width="80%" style="display: block; margin: auto;" />

<img src="./assets/img/sp4-6.png" width="80%" style="display: block; margin: auto;" />

---

## Lecture schedule

1. Drift and variation (Evolution: Chapter 6)
2. Conservation genetics (Evolution: Chapter 6)
3. Phylogeny 1 (Evolution: Chapter 16)
4. **Phylogeny 2 (Evolution: Chapter 16)**

---

## Summary lecture 1

- What a phylogeny is
- Phylogenetics, morphological and genetic data
- **gene trees**
- Uses of phylogenetic trees

## Lecture 2

- key concepts
- How does the gene tree form?
- lineage sorting
- Incomplete lineage sorting
- Gene flow

--- .segue .dark 

## Key concepts

--- &twocol

## Populations and species

*** =left

- A group of individuals capable of reproducing
- Reproduction within populations > between populations
- Ancestral populations diverge creating new populations
- Identified by differences in allele frequencies
- **Species** fulfil the same criteria
- No difference from a population genetics viewpoint

*** =right

<img src="./assets/img/pop1598571799_642096.png" width="75%" style="display: block; margin: auto 0 auto auto;" />

--- &twocol

## Gene tree (single locus tree)

*** =left

- Evolutionary history of a single locus
- (not always an actual gene)
- Each locus has its own gene tree


*** =right

<img src="./assets/img/Gene_Loci_and_Alleles.png" width="75%" style="display: block; margin: auto 0 auto auto;" />

--- &twocol

## Species tree

*** =left

- The **actual** history of populations or species
- Gene trees evolve within the species tree
- May differ due to:
  - **incomplete lineage sorting**
  - **admixture**
- Often what we are trying to infer
  - Concatenation
  - Multispecies coalescent models

*** =right

<img src="./assets/img/gene-tree-incongruence-figure.jpg" width="100%" style="display: block; margin: auto 0 auto auto;" />

--- .segue .dark 

## How does the tree form?

---

## How does the tree form: lineage sorting

<img src="./assets/img/linsort1.svg" width="100%" style="display: block; margin: auto;" />

---

## How does the tree form: lineage sorting

<img src="./assets/img/linsort2.svg" width="100%" style="display: block; margin: auto;" />

---

## How does the tree form: lineage sorting

<img src="./assets/img/linsort3.svg" width="100%" style="display: block; margin: auto;" />

---

## How does the tree form: lineage sorting

<img src="./assets/img/linsort4.svg" width="100%" style="display: block; margin: auto;" />

---

## How does the tree form: lineage sorting

<img src="./assets/img/linsort5.svg" width="100%" style="display: block; margin: auto;" />

---

## Lineage sorting summary

- Drift sorts the lineages into clades
- This takes time, we can't detect the divergence immediately
- We go through stages of incomplete/complete monophyly
- incomplete to complete lineage sorting
- lineage sorting is faster when the population size is small (= more drift)
- Mutation builds upon the clades, monophyly is retained [unless there is gene flow]

**Gene trees may not match the species tree when:**

- We catch the process part way through
- Lineages are not sorted prior to the next divergence/speciation event
- Admixture

--- bg:white

## Big cats

<img src="./assets/img/cats.svg" width="80%" style="display: block; margin: auto;" />

---

## Divergence with complete lineage sorting

<img src="./assets/img/beary1.svg" width="100%" style="display: block; margin: auto;" />

---

## Divergence with complete lineage sorting

<img src="./assets/img/beary2.svg" width="100%" style="display: block; margin: auto;" />

---

## Divergence with complete lineage sorting

<img src="./assets/img/beary3.svg" width="100%" style="display: block; margin: auto;" />

---

## Divergence with complete lineage sorting

<img src="./assets/img/beary4.svg" width="100%" style="display: block; margin: auto;" />

---

## Divergence with complete lineage sorting

<img src="./assets/img/beary5.svg" width="100%" style="display: block; margin: auto;" />

--- .segue .dark 

## What if lineage sorting is incomplete?

---

## Divergence with incomplete lineage sorting

<img src="./assets/img/beary1.svg" width="100%" style="display: block; margin: auto;" />

---

## Divergence with incomplete lineage sorting

<img src="./assets/img/beary2.svg" width="100%" style="display: block; margin: auto;" />

---

## Divergence with incomplete lineage sorting

<img src="./assets/img/ils3.svg" width="100%" style="display: block; margin: auto;" />

---

## Divergence with incomplete lineage sorting

<img src="./assets/img/ils4.svg" width="100%" style="display: block; margin: auto;" />

--- .segue .dark 

## Or...

---

## Divergence with incomplete lineage sorting

<img src="./assets/img/ils3.svg" width="100%" style="display: block; margin: auto;" />

---

## Divergence with incomplete lineage sorting

<img src="./assets/img/ils5.svg" width="100%" style="display: block; margin: auto;" />

---

## Simulator

<iframe src = 'https://heavywatal.github.io/driftr.js/'></iframe>

---

## Summary

- [Note these a just some of the many outcomes you could imagine]
- The danger zone is when alleles fail to reach fixation early in the speciation process
- i.e. prior to SpA population divergence in the example
- Because there is no selection for specific alleles, the process is random
- Either SpA population may end up grouping with SpB

---

## Relying on a single locus tree could be misleading

- Recent divergence with large populations more likely to cause problems
- But no way of easily predicting/testing this from a single tree

### Solution: multiple loci

- Generate data from several loci
- Divide whole genome sequences into loci
- Increased statistical confidence
- Can also quantify ILS (says something about pop size and divergence time)
- Potential to study **gene flow**

--- .segue .dark 

## Multi-locus phylogenetics

--- &twocol

## Brown bear and polar bears

*** =left

<img src="./assets/img/arctos_mt.svg" width="100%" style="display: block; margin: auto;" />

*** =right

<img src="./assets/img/arctos_map.svg" width="100%" style="display: block; margin: auto;" />

- Brown bears not monophyletic
- Divergence time ~120 Ka
- Incomplete lineage sorting (result of recent speciation)?
- Something else?
- Multiple divergent brown bear clades
- Evidence of glacial refugia

--- bg:white

## Brown bear and polar bear Y chromosome

<img src="./assets/img/arctos_y.svg" width="100%" style="display: block; margin: auto;" />

--- &twocol bg:white

## Brown bear and polar bear autosomes

*** =left

<img src="./assets/img/arctos_auto.svg" width="80%" style="display: block; margin: auto;" />

*** =right

- mtDNA suggests recent speciation and brown bear glacial refugia
- Y chromosome suggests species monophyly, no evidence of brown bear refugia
- Autosomes show species monophyly, and that the species are OLD (latest estimates, 1 million years)

### Explanation

- The 2 species are old and distinct
- Males move about more than females
- More recent mtDNA divergence may suggest **gene flow**

--- .segue .dark 

## Detecting gene flow

---

## Divergence with incomplete lineage sorting

<img src="./assets/img/ils3.svg" width="100%" style="display: block; margin: auto;" />

---

## Divergence with incomplete lineage sorting

<img src="./assets/img/ils4 (copy).svg" width="100%" style="display: block; margin: auto;" />

---

## Divergence with incomplete lineage sorting

<img src="./assets/img/ils5 (copy).svg" width="100%" style="display: block; margin: auto;" />

---

## Expected tree frequecies under ILS?

<img src="./assets/img/freq.svg" width="100%" style="display: block; margin: auto;" />

--- .segue .dark 

## What about gene flow?

---

## Speciation with complete lineage sorting

<img src="./assets/img/beary5 (copy).svg" width="100%" style="display: block; margin: auto;" />

---

## Speciation with complete lineage sorting

<img src="./assets/img/bearyG.svg" width="100%" style="display: block; margin: auto;" />

---

## Speciation with complete lineage sorting

<img src="./assets/img/bearyG2.svg" width="100%" style="display: block; margin: auto;" />

---

## Expected tree frequencies with gene flow?

<img src="./assets/img/flow.svg" width="100%" style="display: block; margin: auto;" />

---

## Summary

- An imbalance in the non-species tree topologies provides evidence of gene flow
- Only works if you have sequenced a LOT of loci (whole genomes)
- Can detect very ancient events
- Sometimes based on SNPs (D statistics, F-ratio statistics), essentially the same
- Revealed many examples of gene flow in the past decade


--- &twocol

## Brown bear and polar bears

*** =left

<img src="./assets/img/arctos_mt.svg" width="100%" style="display: block; margin: auto;" />

*** =right

**Nuclear genomes, 100 kb windows**

<img src="./assets/img/abc.svg" width="80%" style="display: block; margin: auto;" />

---

## Brown bear and polar bear reading

<embed src="./assets/img/2015-Genomic_evidence_of_geographically_widespread_effect_of_gene_flow_from_polar_bears_into_brown_bears..pdf" width="100%" height="500" type="application/pdf" />

---

## Brown bear and polar bear reading

<embed src="./assets/img/2014-Brown_and_polar_bear_y_chromosomes_reveal_extensive_male-biased_gene_flow_within_brother_lineages.pdf" width="100%" height="500" type="application/pdf" />

--- &twocol

## Cave bears and brown bears

*** =left

- Cave bears are sister lineage to brown bears and polar bears
- Giant vegan bears
- Extinct ~25 Ka
- Lived alongside brown bears for most of their evolutionary history

*** =right

<img src="./assets/img/kudarensis.png" width="100%" style="display: block; margin: auto;" />

<img src="./assets/img/Ursus_spelaeus_Sergiodlarosa.jpg" width="90%" style="display: block; margin: auto;" />

--- &twocol

## Cave bears and brown bears

*** =left

**Nuclear genomes, 25 kb windows**

<img src="./assets/img/cave_freq.svg" width="80%" style="display: block; margin: auto;" />
*** =right

<img src="./assets/img/kudarensis.png" width="100%" style="display: block; margin: auto;" />

<img src="./assets/img/Ursus_spelaeus_Sergiodlarosa.jpg" width="90%" style="display: block; margin: auto;" />

---

## Cave bear reading

<embed src="./assets/img/Barlow et al. - 2018 - Partial genomic survival of cave bears in living brown bears.pdf" width="100%" height="500" type="application/pdf" />

--- &twocol

## Neanderthals and anatomically modern humans

*** =left

- Extinct population of humans
- Extinct ~40 Ka
- Basically a human (many morphological characters overlapping)
- Advanced culture, hunting technology, art, etc.
- Major dispersal of anatomically modern humans 70-50 Ka
- Population replacement or admixture?

*** =right

<img src="./assets/img/neanderthal_woman-4x3.jpg" width="100%" style="display: block; margin: auto;" />

--- &twocol

## Neanderthals and anatomically modern humans

*** =left

<img src="./assets/img/neander.svg" width="100%" style="display: block; margin: auto;" />

[SNP based analysis, but essentially the same]

*** =right

<img src="./assets/img/neanderthal_woman-4x3.jpg" width="100%" style="display: block; margin: auto;" />

---

## Neanderthal reading

<embed src="./assets/img/2010-A_draft_sequence_of_the_Neandertal_genome..pdf" width="100%" height="500" type="application/pdf" />

--- &thankyou

## Thank you 
