
**Overview Metadata**:      
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

*Required fields are marked with an asterisk, and indicated in detailed tables below.


---

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
|**Format**               |Controlled vocabulary|
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
|**Definition**           |Are data collected continuously or over several discrete time windows|
|**Type**                 |String|
|**Format**               |Controlled vocabulary|
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
