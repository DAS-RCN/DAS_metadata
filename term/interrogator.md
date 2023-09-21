**Interrogator Metadata**
* The Interrogator metadata contains information about the interrogator unit used for the data collection. More than one interrogator may be operating during an experiment, therefore each unit is given a unique identifier and described in individual Interrogator metadata blocks.

* Required fields *(mark with an asterisk, and indicated in the tables below)*
[interrogator_id*](#interrogator_id) |
[manufacturer*](#manufacturer) |
[model*](#model) |

* Optional fields\
[serial_number](#serial_number) |
[firmware_version](#firmware_version) |
[comment](#comment)

---

### interrogator_id
|attributeID              |<div align="right">interrogator_id <img width=200/> <code>Required</code> </div>|
|:------------------------|:----------------------------------------------------|
|**Description**         |Unique identifier of the interrogator unit used in the experiment, assigned by data provider. Identifier should have a maximum of 8 alphanumeric characters with no special characters (e.g., underscores, period, dash). |
|**Required**            |True|
|**Type**                |String|
|**Style**               |Alphanumeric|
|**Units or options**    | -- |
|**Example**             |IU001|

### manufacturer
|attributeID              |<div align="right">manufacturer <img width=200/> <code>Required</code> </div>|
|:------------------------|:----------------------------------------------------|
|**Description**         |Manufacturer name of the interrogator. |
|**Required**            |True|
|**Type**                |String|
|**Style**               |Free form text|
|**Units or options**    | -- |
|**Example**             |Silixa|

### model
|attributeID              |<div align="right">model <img width=200/> <code>Required</code> </div>|
|:------------------------|:----------------------------------------------------|
|**Description**         |Model number of the interrogator. |
|**Required**            |True|
|**Type**                |String|
|**Style**               |Free form text|
|**Units or options**    | -- |
|**Example**             |iDAS|

### serial_number
|attributeID              |<div align="right">serial_number <img width=200/> <code>Optional</code> </div>|
|:------------------------|:----------------------------------------------------|
|**Description**         |Serial number of the interrogator.|
|**Required**            |False|
|**Type**                |String|
|**Style**               |Free form text|
|**Units or options**    | -- |
|**Example**             |16043|

### firmware_version
|attributeID              |<div align="right">firmware_version <img width=200/> <code>Optional</code> </div>|
|:------------------------|:----------------------------------------------------|
|**Description**         |Firmware version of the software used within the interrogator.|
|**Required**            |False|
|**Type**                |String|
|**Style**               |Free form text|
|**Units or options**    | -- |
|**Example**             | -- |

### comment
|attributeID              |<div align="right">comment <img width=200/> <code>Optional</code> </div>|
|:------------------------|:----------------------------------------------------|
|**Description**         |Additional comments.|
|**Required**            |False|
|**Type**                |String|
|**Style**               |Free form text|
|**Units or options**    | -- |
|**Example**             | -- |
