# Distributed Acoustic Sensing Metadata Guide

Here you will find proposed guidelines for standardizing sample metadata to describe interdisciplinary samples within DOE's Environmental Systems Science community.

Most of the sample metadata follows [SESAR's metadata guidelines](http://doi.org/10.5281/zenodo.3874923). However, we modified some metadata elements, specific requirements, and vocabularies based on ESS community needs. This includes additional fields, which mostly come from biodiversity standards [Darwin Core](https://dwc.tdwg.org/), or genomic standards [Minimum Information about any Sequence (MIxS)](https://gensc.org/mixs/). 

We seek any additional feedback, with the goal of making ESS sample information **F**indable, **A**ccessible, **I**nteroperable, and **R**eusable (FAIR). 

---  
## Sample Metadata Content - Link to More Details
*Required fields are marked with an asterisk, and indicated in detailed tables below.

**[Overview](#overview)**:      
[Location*](#location) |
[Deployment type*] (#Deployment-type)



---  
## Overview

### Location
|AttributeID              |<div align="right">location <img width=200/> <code>Required</code> </div>| 
|:------------------------|:----------------------------------------------------|
|**Definition**           |Description of geographic location|
|**Type**                 |String|
|**Format**               |Free form|
|**Additional Instructions**| -- 
|**Examples**             |Parkfield, California, USA|

### Deployment-type
|AttributeID              |<div align="right">deployment_type <img width=200/> <code>Required</code> </div>| 
|:------------------------|:----------------------------------------------------|
|**Definition**           |Describes the permenancy of the deployment|
|**Type**                 |String|
|**Format**               |Controlled Vocabulary|
|**Options**              |[permanent , temporary]|
|**Additional Instructions**| -- 
|**Examples**             |permanent|





