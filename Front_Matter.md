---
title: Cybersecurity Considerations for Heavy Vehicle Event Data Recorders
subtitle: TARA Report
author:
- Ben Gardiner, ben.gardiner@irdeto.com
- Jeremy S. Daily, jeremy-daily@utulsa.edu
date: 1 June 2018
...

# Introduction

This report is generated [^aa] from an attack tree threat (and fault) model developed for the esCAR 2018 paper, *Cybersecurity Considerations for Heavy Vehicle Event Data Recorders*.

[^aa]: generated using the [mindmup-as-attack-trees tool](https://github.com/BenGardiner/mindmup-as-attack-trees)

# Executive Summary

The threats facing digital forensic data were presented as an attack tree to create a comprehensive list of mitigations for the end threat where HVEDR data is presented that does not accurately represent the physical phenomena under question. The threat model covers the acquisition, transfer, storage, and verification of the data. It also addresses scaling and offset issues when converting digital data in to scaled engineering units, but verifying trust the data values requires testing and comparison to external reference measurements.

The analysis revealed, for example, that increased attack surface through vehicle connectivity solutions can increase the burdens on the forensic investigator to address potential alteration of data in different phases of the forensic process. Current processes of using local connections with diagnostic software may lack high assurance methods to maintain data integrity. The attack trees show 28 different potential attack vectors or error conditions, some of them impractical, but others much more realistic.

Once the threats were enumerated, mitigation strategies were proposed. The model places the mitigations in the context of which attacks or error conditions that they will mitigate. For example, by simply signing forensic data at the time of acquisition with cryptographically sound techniques, like the Pretty Good Privacy (PGP) framework, will mitigate the risk of altering data records after download and will do so on vehicle networks deployed today.

Note: in a complete TARA, where the impacts to stakeholders of multiple attacker objectives are well understood and modeled with fidelity, this location in the *Executive Summary* would list the most impactful mitigations. In the case of this generated report, such a model of impacts is not available. See also the section *A Note About the Following EVITA Risk Analysis* for more details.

These mitigations (or equivalently thought of as security requirements), if deployed correctly, could alleviate the burden on the investigator to maintain high assurance of the digital forensic data. This paper expanded on what security requirements are needed to ensure the continued high assurance of the forensic data extraction process. Some technologies, mechanisms, designs or techniques would be sufficient for these security requirements; but no specific solutions are proposed as implementations of the requirements and additional solutions are not only possible, but encouraged.

Digital forensic data from heavy vehicles is critical in determining crash causation and the trust in this data is paramount. Improving the cybersecurity controls on this forensic data is necessary for society to adopt more data-driven technologies such as autonomous operations.

