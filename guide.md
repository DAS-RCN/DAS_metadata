# Distributed Acoustic Sensing Metadata Guide

Here you will find proposed guidelines for standardizing DAS metadata for archival purposes and to guide data collection at experiments. The intent is that this metadata data standard should be independent of the specific implementation and the emphasis is on content. We provide a suggested outline for content and show examples for several case studies.

In addition, we distinguish between required and recommended metadata.  Required metadata is information that is considered essential to enable re-use of the data. This information makes the data self-describing and no further information required from the provider to work with the data. Optional metadata is information that could be useful in interpreting the measured signal but is not essential. For example, gauge length is required metadata while the geographic coordinates of tap tests used to provide gauge positions is recommended. 

We seek any additional feedback, with the goal of making DAS products **F**indable, **A**ccessible, **I**nteroperable, and **R**eusable (FAIR). 

---  
## Metadata Content 
*Required fields are marked with an asterisk, and indicated in detailed tables below.

**[Overview Metadata](#overview-metadata)**:      
[Location*](#location) |
[Deployment type*](#deployment-type) |
[Network*](#network) |
[Site name*](#site-name) |
[Number_of_interrogators*](#number-of-interrogators) |
[Principle investigators*](#principle-investigators) |
[Start datetime*](#start-datetime) |
[End datetime*](#end-datetime) |
[Purpose of collection](#purpose-of-collection) |
[Collection mode](#collection-mode) |
[Comment](#comment) |

**[Cable and Fiber Metadata](#cable-and-fiber-metadata)**:      
[Cable fiber ID*](#cable-fiber-ID) |
[Cable start time](#cable-start-time) |
[Cable end time](#cable-end-time) |
[Cable characteristics](#cable-characteristics) |

**[Interrogator Metadata](#interrogator-metadata)**: 

**[Acquisition Metadata](#acquisition-metadata)**: 

**[Channel Metadata](#channel-metadata)**: 

---  
## Overview Metadata

### Location
|AttributeID              |<div align="right">location <img width=200/> <code>Required</code> </div>| 
|:------------------------|:----------------------------------------------------|
|**Definition**           |Description of geographic location|
|**Type**                 |String|
|**Format**               |Free form|
|**Additional Instructions**| -- 
|**Examples**             |Parkfield, California, USA|

### Deployment type
|AttributeID              |<div align="right">deployment_type <img width=200/> <code>Required</code> </div>| 
|:------------------------|:----------------------------------------------------|
|**Definition**           |Describes the permenancy of the deployment|
|**Type**                 |String|
|**Format**               |Controlled Vocabulary|
|**Options**              |[permanent , temporary]|
|**Additional Instructions**| -- 
|**Examples**             |permanent|

### Network
|AttributeID              |<div align="right">network <img width=200/> <code>Required</code> </div>| 
|:------------------------|:----------------------------------------------------|
|**Definition**           |A network name that is managed by an organization accepted by the international community. The network name should uniquely identify the the source of the data|
|**Type**                 |String|
|**Format**               |Alpha Numeric|
|**Additional Instructions**| -- 
|**Examples**             |PB|

### Site name
|AttributeID              |<div align="right">site_name <img width=200/> <code>Required</code> </div>| 
|:------------------------|:----------------------------------------------------|
|**Definition**           |Name of data collection site|
|**Type**                 |String|
|**Format**               |Free form|
|**Additional Instructions**| -- 
|**Examples**             |SAFOD Borehole|

### Number of interrogators
|AttributeID              |<div align="right">number_of_interrogators <img width=200/> <code>Required</code> </div>| 
|:------------------------|:----------------------------------------------------|
|**Definition**           |Number of interrogators used to collect data over the course of data collection|
|**Type**                 |Integer|
|**Additional Instructions**| -- 
|**Examples**             |2|

### Principle investigators
|AttributeID              |<div align="right">principle_investigators <img width=200/> <code>Required</code> </div>| 
|:------------------------|:----------------------------------------------------|
|**Definition**           |Point of Contact(s)|
|**Type**                 |String|
|**Additional Instructions**| -- 
|**Examples**             |P.I. Doe|

### Start datetime
|AttributeID              |<div align="right">start_datetime <img width=200/> <code>Required</code> </div>| 
|:------------------------|:----------------------------------------------------|
|**Definition**           |Start date of experiment|
|**Type**                 |String|
|**Format**               |ISO formatted date-time|
|**Unit**                 |UTC|
|**Additional Instructions**| -- 
|**Examples**             |2018-02-11T00:00:00|

### End datetime
|AttributeID              |<div align="right">end_datetime <img width=200/> <code>Required</code> </div>| 
|:------------------------|:----------------------------------------------------|
|**Definition**           |End date of experiment|
|**Type**                 |String|
|**Format**               |ISO formatted date-time|
|**Unit**                 |UTC|
|**Additional Instructions**| -- 
|**Examples**             |2018-03-24T00:00:00|

### Purpose of collection
|AttributeID              |<div align="right">purpose_of_collection <img width=200/> <code>Optional</code> </div>| 
|:------------------------|:----------------------------------------------------|
|**Definition**           |Brief explanation of purpose|
|**Type**                 |String|
|**Format**               |Free form|
|**Additional Instructions**| -- 
|**Examples**             |Ambient noise study|

### Collection mode
|AttributeID              |<div align="right">collection_mode <img width=200/> <code>Optional</code> </div>| 
|:------------------------|:----------------------------------------------------|
|**Definition**           |Are data collected continuously or over several  discrete time windows|
|**Type**                 |String|
|**Format**               |Controlled Vocabulary|
|**Options**              |[continuous, segmented]|
|**Additional Instructions**| -- 
|**Examples**             |continuous|

### Comment
|AttributeID              |<div align="right">comment <img width=200/> <code>Optional</code> </div>| 
|:------------------------|:----------------------------------------------------|
|**Definition**           |Add additional comment|
|**Type**                 |String|
|**Format**               |Free form|
|**Additional Instructions**| -- 
|**Examples**             |--|

---
## Cable and Fiber Metadata

### Cable fiber ID
|AttributeID              |<div align="right">cable_fiber_id <img width=200/> <code>Required</code> </div>| 
|:------------------------|:----------------------------------------------------|
|**Definition**           |A term that identifies the fiber used within an experiment, e.g., alpha-numeric code defined by the researcher, default = 1|
|**Type**                 |String|
|**Format**               |Alpha Numeric|
|**Default**              |1|
|**Additional Instructions**| -- 
|**Examples**             |1A|

### Cable start time
|AttributeID              |<div align="right">cable_start_time <img width=200/> <code>Optional</code> </div>| 
|:------------------------|:----------------------------------------------------|
|**Definition**           |Installation time of the cable|
|**Type**                 |String|
|**Format**               |ISO formatted date-time|
|**Unit**                 |UTC|
|**Additional Instructions**| -- 
|**Examples**             |2012-12-14T00:00:00|

### Cable end time
|AttributeID              |<div align="right">cable_end_time <img width=200/> <code>Optional</code> </div>| 
|:------------------------|:----------------------------------------------------|
|**Definition**           |Removal of the cable|
|**Type**                 |String|
|**Format**               |ISO formatted date-time|
|**Unit**                 |UTC|
|**Additional Instructions**| -- 
|**Examples**             |22013-02-24T00:00:00|

### Cable characteristics
|AttributeID              |<div align="right">cable_characteristics <img width=200/> <code>Optional</code> </div>| 
|:------------------------|:----------------------------------------------------|
|**Definition**           |Describes how the fiber is encased in the cable|
|**Type**                 |String|
|**Format**               |Controlled Vocabulary|
|**Options**              |[buffered, armored, gel-filled]|
|**Additional Instructions**| -- 
|**Examples**             |gel-filled|

### Cable environment
|AttributeID              |<div align="right">cable_characteristics <img width=200/> <code>Optional</code> </div>| 
|:------------------------|:----------------------------------------------------|
|**Definition**           |describes the installation environment|
|**Type**                 |String|
|**Format**               |Controlled Vocabulary|
|**Options**              |[[Conduit, trench, outside borehole casing, wireline]|
|**Additional Instructions**| -- 
|**Examples**             |outside borehole casing|
