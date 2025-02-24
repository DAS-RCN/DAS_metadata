## DAS-RCN Reporting Format for Distributed Acoustic Sensing (DAS) metadata v1.1.0

Distributed Acoustic Sensing (DAS) is a transformative technology and its applications in geosciences and engineering are numerous and growing. To move this frontier technology forward, it is important to compare and integrate measurements across deployments and make the data reusable by others following Findable, Accessible, Interoperable, and Reusable (FAIR) data principles (Wilkinson et al., 2016). Long-standing metadata standards such as the Standard for the Exchange of Earthquake Data (SEED) (Ahern et al., 2009) developed for seismic data do not adapt well for DAS due to fundamental differences in sensor and data acquisition parameters. Existing formats for seismic metadata developed in the early days of digital seismic recording, such as dataless SEED and SEG-Y headers, cannot accommodate all the acquisition parameters, cable environment, and channel location information needed for proper characterization.

Here, DAS-RCN Data Management Working Group presents ***DAS metadata standard*** (v1.1.0), specifically for DAS research community to facilitate the integration of DAS measurements across experiments and increase reusability. This standard V1.1.0 (improved from V1.0.0) fully describes the five key components of a DAS experiment: interrogator, data acquisition, channels, cable, and fiber. The intent is that this metadata standard should be independent of the specific implementation and the emphasis is on the content and structure (i.e., schema). This also implies that the metadata is independent of the time-series data. 

**⚠️ (Feb 24, 2025) This repository has been archived and is no longer maintained. Please visit the [FDSN DAS metadata github respository](https://github.com/FDSN/DAS-metadata) for updates and issue tracking. ⚠️**

--- 

## Getting started  

0. Optional to use our reader-friendly website [url](https://das-metadata.gitbook.io/das-metadata-standard-by-das-rcn/)
1. Read the DAS metadata [terms and definitions](./term/README.md)
2. Download [templates](./template/README.md) for the standardized attributes
3. Explore our [example gallery](./example/README.md) for DAS metadata in different deployment scenarios.

## How to contribute  

Want to make a change to the reporting format? 

Submit a new issue [here](https://github.com/vhlai-seis/DAS_metadata/blob/main/contribute.md) and use one of several templates that we provide to: 
- suggest a new term
- modify a term
- propose changes to documentation within this repository
- request features 
- report bugs

---

## Version history 

### February 24, 2025
This repository has been archived and is no longer actively maintained. All future updates, developments, and issue tracking will take place in the FDSN repository: [https://github.com/FDSN/DAS-metadata](https://github.com/FDSN/DAS-metadata).

Please direct any new issues or contributions there. Thank you for your support.

### v1.1.0 (September 21, 2023)

This updated DAS Metadata Schema introduces significant changes, including the creation of distinct child branches for Cable (and Fiber) and for Interrogator (including Acquisition, Channel Group, and Channel).
Subsequent modifications to the GitHub repository consist of minor editorial edits with no major structural or functional changes.

Citation: 
- [journal article] Voon-Hui Lai, Kathleen M. Hodgkinson, Robert W. Porritt, Robert Mellors; Toward a Metadata Standard for Distributed Acoustic Sensing (DAS) Data Collection. Seismological Research Letters 2024;; 95 (3): 1986–1999. doi: https://doi.org/10.1785/0220230325 

### v1.0.0 (August 24, 2022)

Initial release of the DAS Metadata Reporting Format developed by the DAS Research Coordination Network Data Management Working Group.
The schema and framework were outlined in an accompanying white paper (unpublished, no DOI) and supported by two conference presentations.

References:
- [White paper] Mellors, Rob, Hodgkinson, Kathleen, Lai, Voon Hui, and DAS Data Management Working Group. Distributed Acoustic Sensing (DAS) Metadata Model. May 5, 2022
- [Conference paper] Mellors, Rob, Hodgkinson, Kathleen, Lai, Voon Hui, and DAS Data Management Working Group. Initial steps towards a DAS metadata model. United States: N. p., 2022. Web. doi:10.2172/2002283.
- [Conference paper] Hodgkinson, Kathleen Marian, Lai, Voon Hui, Mellors, Robert J., Porritt, Robert William, and Stanciu, Adrian Christian. A Metadata Exchange Model for Distributed Acoustic Sensing (DAS). United States: N. p., 2023. Web. doi:10.2172/2432128.

--- 

## Copyright information  

The DAS-RCN Reporting Format for DAS metadata is licensed under the Creative Commons Attribution 4.0 International (CCby4).

## Funding and acknowledgements  

The team (Voon Hui Lai, Kathleen Hodgkinson, Robert Porritt, Robert Mellors) would like to thank all who provided input and in particular, members of the DAS RCN Metadata working group: Jonathan Ajo-Franklin; Kent Anderson; Sandra Barajas; Paul Bodin; Jerry Carter; Luigia Cristiano; Ben Evans; Ge Jin; Meghan Miller; Helle Pedersen; Javier Quinteros; Nigel Rees; Diane Rivet; Jonathan Schaeffer; Nicole Taverna; Chad Trabant; Arantza Ugalde; Antonio Villaseñor; Jon Weers; Ray Willemann; Lesley Wyborn; Nate Lindsey; Zack Spica; Andreas Wuestefeld. We would also like to specially acknowledge Dan Auerbach, Marius Isken, Julián Pelaez, Earthscope Consortium (formally IRIS) Data Management Center for their extensive input and suggestions in improving this metadata standard.

Sandia National Laboratories is a multimission laboratory managed and operated by National Technology & Engineering Solutions of Sandia, LLC, a wholly owned subsidiary of Honeywell International Inc., for the U.S. Department of Energy’s National Nuclear Security Administration under contract DE-NA0003525.

KMH and RWP were supported by the Source Physics Experiment. The Source Physics Experiment (SPE) would not have been possible without the support of many people from several organizations. The authors wish to express their gratitude to the National Nuclear Security Administration, Defense Nuclear Nonproliferation Research and Development (DNN R&D), and the SPE working group, a multi-institutional and interdisciplinary group of scientists and engineers.

## Recommended citation  

Voon-Hui Lai, Kathleen M. Hodgkinson, Robert W. Porritt, Robert Mellors; Toward a Metadata Standard for Distributed Acoustic Sensing (DAS) Data Collection. Seismological Research Letters 2024;; 95 (3): 1986–1999. doi: https://doi.org/10.1785/0220230325



