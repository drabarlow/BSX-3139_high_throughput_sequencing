---
title       : "High throughput sequencing"
subtitle    : "BSX-3139 Molecular Ecology and Evolution"
author      : Dr Axel Barlow
job         : "email: a.barlow.@bangor.ac.uk"
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

## High throughput sequencing

- First generation sequencing (Sanger)
- Second generation sequencing (Illumina)
- Third generation sequencing (PacBio and Oxford Nanopore)

---

## High throughput sequencing

<img src="./assets/img/sequencers.svg" title="plot of chunk unnamed-chunk-1" alt="plot of chunk unnamed-chunk-1" width="95%" style="display: block; margin: auto;" />

---

## High throughput sequencing

<img src="./assets/img/2021_Sequencing_cost_per_Mb.jpg" title="plot of chunk unnamed-chunk-2" alt="plot of chunk unnamed-chunk-2" width="95%" style="display: block; margin: auto;" />

--- .segue .dark 

## First generation sequencing

--- bg:white

## Sanger sequencing

<img src="./assets/img/sanger_gel.svg" title="plot of chunk unnamed-chunk-3" alt="plot of chunk unnamed-chunk-3" width="60%" style="display: block; margin: auto;" />

--- bg:white

## Sanger sequencing

<img src="./assets/img/sanger_auto.svg" title="plot of chunk unnamed-chunk-4" alt="plot of chunk unnamed-chunk-4" width="60%" style="display: block; margin: auto;" />

--- &twocol

## Sanger overview

*** =left

<img src="./assets/img/abi_3130.svg" title="plot of chunk unnamed-chunk-5" alt="plot of chunk unnamed-chunk-5" width="100%" style="display: block; margin: auto;" />

*** =right

- 700-1000 bp
- High accuracy
- 384 samples
- 1 day
- Dominated for 3 decades

--- .segue .dark 

## Second generation sequencing

---

## Illumina

<img src="./assets/img/illumina.svg" title="plot of chunk unnamed-chunk-6" alt="plot of chunk unnamed-chunk-6" width="100%" style="display: block; margin: auto;" />

---

## Data output

Platform | read pairs | Read length | data output | Genome coverage
---|---|---|---|---
MiniSeq|25 million|2 x 150 bp|7.5 Gb|2 x
MiSeq|25 million|2 x 300 bp|15 Gb|4 x
NextSeq 550|400 million|2 x 150 bp|120 Gb|33 x
NextSeq 2000|900 million|2 x 300 bp|540 Gb|150 x
HiSeq X|6 billion|2 x 150 bp|1.8 Tb|500 x
NovaSeq X Plus|52 billion|2 x 150 bp|16 Tb*|4444 x

- *16 Tb = 16,000,000,000,000 bp

---

## Sequencing by synthesis

1. Sample preparation
2. Bind DNA to flowcell, generate clusters
3. Sequencing by synthesis
4. Data analysis (in the machine)

---

## Sample preparation

<img src="./assets/img/library_molecule.svg" title="plot of chunk unnamed-chunk-7" alt="plot of chunk unnamed-chunk-7" width="100%" style="display: block; margin: auto;" />

*Indexes allow multiple samples to be sequenced at the same time

---

## Flow cell

<img src="./assets/img/flowcell2.svg" width="100%" style="display: block; margin: auto;" />

--- bg:white

## Cluster generation

<img src="./assets/img/cluster.svg" title="plot of chunk unnamed-chunk-9" alt="plot of chunk unnamed-chunk-9" width="70%" style="display: block; margin: auto;" />

--- bg:white

## Sequencing by synthesis

<img src="./assets/img/sbs.svg" title="plot of chunk unnamed-chunk-10" alt="plot of chunk unnamed-chunk-10" width="100%" style="display: block; margin: auto;" />

--- bg:white

## Data analysis (in the machine)

<img src="./assets/img/dataanalysis.svg" title="plot of chunk unnamed-chunk-11" alt="plot of chunk unnamed-chunk-11" width="85%" style="display: block; margin: auto;" />

---

## What do we sequence?

[Not an exhaustive list]

- **Whole genome resequencing (pure DNA sample from a single individual)**
- Reduced representation genome data (RADseq, targeted SNPs, single individual)
- Poolseq (multiple individuals)
- Transcriptome (RNA sample from single tissue/individual)
- Metabarcoding (PCR amplicon, multiple individuals/species)
- Metagenomics (whole genomes, multiple individuals/species)

--- &twocol

## Whole genome resequencing

*** =left

- Sequencing reads mapped to an existing **reference genome**
- Easy to identify SNPs relative to reference, and to other samples
- Accuracy depends on the number of reads in the stack, termed **depth** or **coverage**

*** =right

<img src="./assets/img/resequencing.svg" width="80%" style="display: block; margin: auto;" />

---

## Whole genome resequencing

<img src="./assets/img/Screenshot from 2022-09-08 13-58-44.png" title="plot of chunk unnamed-chunk-13" alt="plot of chunk unnamed-chunk-13" width="100%" style="display: block; margin: auto auto auto 0;" />

---

## Example: leopard population genomics

<img src="./assets/img/leopar_res.svg" title="plot of chunk unnamed-chunk-14" alt="plot of chunk unnamed-chunk-14" width="100%" style="display: block; margin: auto auto auto 0;" />

*Paijmans et al. 2021. Current Biology*

---

## Illumina summary

- The current market leader
- Massive output
- **But keep an eye on Ultima Genomics**
- High accuracy
- Many applications (genome resequencing, RADseq, transcriptomes, metabarcoding)
- Cheap (£9 per Gb)
- Major limitation is the read length
- Unsuitable for assembly of reference genomes

--- .segue .dark 

## Third generation sequencing

--- bg:white

## PacBio

<img src="./assets/img/revio_right_closed.jpg" width="100%" style="display: block; margin: auto;" />

--- bg:white

## Single Molecule, Real-Time (SMRT) sequencing

<img src="./assets/img/smrt_seq.svg" alt="plot of chunk unnamed-chunk-16" width="100%" style="display: block; margin: auto;" />

--- 

## HiFi reads

<img src="./assets/img/HiFi-reads-img.svg" alt="plot of chunk unnamed-chunk-17" width="100%" style="display: block; margin: auto;" />

---

## PacBio summary

- Single molecule sequencing (no cluster generation)
- Long reads (around 25 kb)
- 75 Gb per SMRT Cell for Revio
- Fantastic for **assembly of reference genomes**
- Historically high sequencing error, solved by HiFi sequencing
- Still more expensive than Illumina (~£3k per SMRT cell with library prep) 
- Price falling rapidly

---

## What can we do with the data?

<img src="./assets/img/41586_2018_Article_BFnature25458_Fig1_HTML.webp" alt="plot of chunk unnamed-chunk-18" width="100%" style="display: block; margin: auto auto auto 0;" />

*Nowoshilow et al. 2018. Nature*

---

## Oxford Nanopore

<img src="./assets/img/nanopore.svg" width="100%" style="display: block; margin: auto auto auto 0;" />

--- bg:white

## How it works

<img src="./assets/img/ont-sequencing_yourgenome.png" alt="plot of chunk unnamed-chunk-20" width="90%" style="display: block; margin: auto auto auto 0;" />

---

## Field based sequencing

<img src="./assets/img/41586_2016_Article_BFnature16996_Fig1_HTML.webp" alt="plot of chunk unnamed-chunk-21" width="65%" style="display: block; margin: auto auto auto 0;" />

*Quick et al. 2016. Real-time, portable genome sequencing for Ebola surveillance. Nature*

---

## Oxford Nanopore summary

- Variable output, up to Tb's with larger platforms
- Long reads, record is 2.3 Mb!
- Output 20-30 Gb (up to 50 Gb) per Minion flow cell
- High error rate, currently 5-10 % but improving
- Still more expensive than Illumina and PacBio (~£750 for Minion flow cell and library prep)
- True portability and real time sequencing/analysis
- But need to buy sequencer: Minion £4,650 inc. 5 flow cells

---

## Recommended reading

<embed src="./assets/img/Illumina Inc - 2013 - Illumina Sequencing Technology - YouTube.pdf" title="plot of chunk unnamed-chunk-22" width="100%" height="500" type="application/pdf" />

---

## Recommended reading

<embed src="./assets/img/Hu et al. - 2021 - Next-generation sequencing technologies An overview.pdf" title="plot of chunk unnamed-chunk-23" width="100%" height="500" type="application/pdf" />

---

## Recommended reading

<embed src="./assets/img/Athanasopoulou et al. - 2022 - Third-Generation Sequencing The Spearhead towards the Radical Transformation of Modern Genomics.pdf" title="plot of chunk unnamed-chunk-24" width="100%" height="500" type="application/pdf" />

--- &thankyou

## Next time:

**Gene trees and molecular dating**
