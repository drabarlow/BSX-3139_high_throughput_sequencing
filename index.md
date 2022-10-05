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

Platform | Million reads | Read length | Gb data | Genome coverage
---|---|---|---|---
MiniSeq|25|2 x 150 bp|7.5|2
MiSeq|25|2 x 300 bp|15|4
NextSeq|400|2 x 150 bp|120|33
HiSeq X|6000|2 x 150 bp|1800|500
NovaSeq|20000|2 x 150 bp|6000|1667

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

<img src="./assets/img/flowcell.svg" title="plot of chunk unnamed-chunk-8" alt="plot of chunk unnamed-chunk-8" width="80%" style="display: block; margin: auto;" />

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

- **Whole genome sequencing (pure DNA sample from a single individual)**
- Reduced representation genome data (RADseq, targeted SNPs, single individual)
- Poolseq (multiple individuals)
- Transcriptome (RNA sample from single tissue/individual)
- Metabarcoding (PCR amplicon, multiple individuals/species)
- Metagenomics (whole genomes, multiple individuals/species)

---

## Whole genome sequencing

Short reads from a single individual can be mapped to a reference genome assembly

<img src="./assets/img/pseudohap.svg" title="plot of chunk unnamed-chunk-12" alt="plot of chunk unnamed-chunk-12" width="95%" style="display: block; margin: auto;" />

---

## Whole genome sequencing

<img src="./assets/img/Screenshot from 2022-09-08 13-58-44.png" title="plot of chunk unnamed-chunk-13" alt="plot of chunk unnamed-chunk-13" width="100%" style="display: block; margin: auto auto auto 0;" />

---

## Example: leopard population genomics

<img src="./assets/img/leopar_res.svg" title="plot of chunk unnamed-chunk-14" alt="plot of chunk unnamed-chunk-14" width="100%" style="display: block; margin: auto auto auto 0;" />

*Paijmans et al. 2021. Current Biology*

---

## Illumina summary

- The current market leader
- Massive output
- Many applications (genome resequencing, RADseq, transcriptomes, metabarcoding)
- Cheap (£10 per Gb)
- Major limitation is the read length

--- .segue .dark 

## Third generation sequencing

---

## PacBio

<img src="./assets/img/sequel-2Bimage.jpg" alt="plot of chunk unnamed-chunk-15" width="50%" style="display: block; margin: auto;" />

--- bg:white

## Single Molecule, Real-Time (SMRT) sequencing

<img src="./assets/img/smrt_seq.svg" alt="plot of chunk unnamed-chunk-16" width="100%" style="display: block; margin: auto;" />

--- 

## HiFi reads

<img src="./assets/img/HiFi-reads-img.svg" alt="plot of chunk unnamed-chunk-17" width="100%" style="display: block; margin: auto;" />

---

## PacBio summary

- Single molecule sequencing (no cluster generation)
- Long reads (up to 50 kb)
- Fantastic for **genome assemblies**
- Historically high sequencing error, solved by HiFi sequencing

---

## What can we do with the data?

<img src="./assets/img/41586_2018_Article_BFnature25458_Fig1_HTML.webp" alt="plot of chunk unnamed-chunk-18" width="100%" style="display: block; margin: auto auto auto 0;" />

*Nowoshilow et al. 2018. Nature*

---

## Oxford Nanopore

<img src="./assets/img/Oxford Nanopore devices.png" alt="plot of chunk unnamed-chunk-19" width="100%" style="display: block; margin: auto auto auto 0;" />

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
- High error rate, currently 5-10 % but improving
- Portability and real time sequencing/analysis

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
