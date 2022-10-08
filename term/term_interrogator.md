**[Interrogator](#interrogator-metadata)**
* Contains information about the interrogators used. More than one interrogator may be operating during an experiment. Each interrogator is described in one interrogator metadata block. The metadata consists of a unique identifier, the interrogator model, and the unit of measure.

* Required fields *(mark with an asterisk, and indicated in the tables below)*  
[Interrogator ID*](#interrogator-ID) |
[Manufacturer*](#manufacturer) |
[Model*](#model) |
[Unit of measure*](#unit-of-measure) 


---

### Interrogator ID
|AttributeID              |<div align="right">interrogator_id <img width=200/> <code>Required</code> </div>| 
|:------------------------|:----------------------------------------------------|
|**Definition**           |The Interrogator ID uniquely identifies the interrogator used within the network. User defined. |
|**Type**                 |String|
|**Format**               |Alpha numeric|
|**Additional Instructions**| -- 
|**Examples**             |1|

### Manufacturer
|AttributeID              |<div align="right">manufacturer <img width=200/> <code>Required</code> </div>| 
|:------------------------|:----------------------------------------------------|
|**Definition**           |Interrogator manufacturer  |
|**Type**                 |Text|
|**Format**               |Free form|
|**Additional Instructions**| -- 
|**Examples**             |Silixa|

### Model
|AttributeID              |<div align="right">model <img width=200/> <code>Required</code> </div>| 
|:------------------------|:----------------------------------------------------|
|**Definition**           |A model number or name that uniquely identifies the interrogator   |
|**Type**                 |Text|
|**Format**               |Free form|
|**Additional Instructions**| -- 
|**Examples**             |iDAS 123|

### Unit of measure
|AttributeID              |<div align="right">unit_of_measure <img width=200/> <code>Required</code> </div>| 
|:------------------------|:----------------------------------------------------|
|**Definition**           |Interrogators natural unit of measure|
|**Type**                 |String|
|**Format**               |Controlled vocabulary|
|**Options**              |[natural units, strain, strain-rate, velocity]|
|**Additional Instructions**| -- 
|**Examples**             |strain-rate|
