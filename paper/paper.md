---
title: 'BioHackJP 2023 Report R4: integration of glyco data with chemo-, geno-, lipid-omics and pathway data'
title_short: 'BioHackJP 2023 Glyco'
tags:
  - Glycoscience
  - Chemoinformatics
  - Proteins
  - Lipids
  - Gene variants
authors:
  - name: Kiyoko F. Aoki-Kinoshita
    orcid: 0000-0002-6662-8015
    affiliation: 1
  - name: Evan Bolton
    orcid: 0000-0002-5959-6190
    affiliation: 2
  - name: Issaku Yamada
    orcid: 0000-0001-9504-189X
    affiliation: 3
  - name: Akihiro Fujita
    orcid: 0000-0003-3748-7791
    affiliation: 1
affiliations:
  - name: Soka University
    index: 1
  - name: National Center for Biotechnolog Information (NCBI), PubChem
    index: 2
  - name: The Noguchi Institute
    index: 3
date: 30 June 2023
cito-bibliography: paper.bib
event: BH23JP
biohackathon_name: "BioHackathon Japan 2023"
biohackathon_url:   "https://2023.biohackathon.org/"
biohackathon_location: "Kagawa, Japan, 2023"
group: R4
# URL to project git repo --- should contain the actual paper.md:
git_url: https://github.com/biohackathon-japan/bh23-glyco
# This is the short authors description that is used at the
# bottom of the generated paper (typically the first two authors):
authors_short: Kiyoko F. Aoki-Kinoshita \emph{et al.}
---

# Background

# Outcomes

## Integration of glycan data from GlyTouCan with PubChem

### update GlyTouCan data

In order to smooth integration, we decided to commence with the forthcoming release of the GlyTouCan data. Then, we updated the GlyTouCan data by utilizing the latest WURCSFramework.

### Exhaustive analysis for PubChem structures to detect sugars using MolWURCS and Sugar'n'Splice
To integrate glycan data between PubChem and GlyTouCan, we have developed a software tool, MolWURCS, for extracting sugars, including monosaccharides and glycans, from chemical structure fomulae as WURCS. In this time, we performed exhaustive analysis for all data in PubChem and GlyTouCan using MolWURCS. To complement and compare the result of the sugar detection, we also used the result of Sugar'n'Splice which detects not only sugars but also the other biopolymers including nucleic acids and amino acids.

The analysis can be separated into the followings:
- MW vs SNS: Comparison of the results between MolWURCS (MW) and Sugar'n'Splice (SNS)
  - To updating the accuracy of sugar detection by comparing the results between MolWURCS (MW) and Sugar'n'Splice (SNS) in PubChem
- Identifying and analyzing failure cases in conversion between WURCS and MOL/SDF in PubChem and GlyTouCan
  - To improve MolWURCS performance to integrate glycan data

The document then presents several datasets and analysis results:

MW vs SNS:

Datasets include PubChem CID to WURCS conversions and unique CID and WURCS lists.
Analysis includes comparing unique structures and identifying common and unique entries between MW and SNS glycan and biologic datasets.

PubChem-MolWURCS:

Datasets involve PubChem to MolWURCS conversions, WURCS to MOL/SDF conversions, and analysis of successes and failures in conversion.
Various reasons for failure are identified and categorized.

GlyTouCan-MolWURCS:

Datasets cover GlyTouCan WURCS to WURCS validation conversions and WURCS to MOL/SDF conversions.
Analysis includes the success and failure rates of conversions, along with reasons for failures.
Throughout the document, links to specific datasets and analysis results are provided.

## Integration of glycan data from GlyCosmos with UniProt

## Investigation of glycogene variants and phenotypes to integrate with GlyCosmos


![Caption for BioHackrXiv logo figure](./biohackrxiv.png)

# Future work

## Annotating entries in PubChem that contain glycans

## Integration of variant data into GlyCosmos


## Acknowledgements

We would like to thank the fellow participants at BioHackathon 2023 for their collaboration and constructive advice, which greatly influenced our project. We are grateful to the organizers for providing this platform and the developers of open source language models. Special thanks to our mentors, advisors, and colleagues for their guidance and support. Without their contributions, our project in linked data standardization with LLMs in bioinformatics would not have been possible.

## References

1.
