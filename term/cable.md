**Cable Metadata**
*  The Cable metadata is designed to allow investigators to describe the cable used in their experiment, which could be one continuous long cable, or cables with multiple connectors or across several installation environments. There are also parameters relating to the general geographical location of the cable to facilitate searchability in future databases. The Cable metadata should include available information on the cable and its installation as this knowledge may help in developing a system-level description of the exact cable response.

* Required fields *(mark with an asterisk, and indicated in the tables below)* \
[cable_id*](#cable_id) |
[cable_bounding_box*](#cable_bounding_box) 


* Optional fields\
[cable_owner](#cable_owner) |
[cable_installation_date](#cable_installation_date) |
[cable_removal_date](#cable_removal_date) |
[cable_characteristics](#cable_characteristics) |
[cable_environment](#cable_environment) |
[cable_installation_environment](#cable_installation_environment) |
[cable_model](#cable_model) |
[cable_outside_diameter](#cable_outside_diameter) |
[cable_outside_diameter_unit](#cable_outside_diameter_unit) |
[comment](#comment)

---

### cable_id
|attributeID              |<div align="right">cable_id <img width=200/> <code>Required</code> </div>|
|:------------------------|:----------------------------------------------------|
|**Description**         |Unique identifier for the specific physical cable used in the data acquisition. Identifier should have a maximum of 8 alphanumeric characters with no special characters (e.g., underscores, period, dash). |
|**Required**            |True|
|**Type**                |String|
|**Style**               |Alphanumeric|
|**Units or options**    | -- |
|**Example**             |CA001|

### cable_bounding_box
|attributeID              |<div align="right">cable_bounding_box <img width=200/> <code>Required</code> </div>|
|:------------------------|:----------------------------------------------------|
|**Description**         |List of approximate coordinates of the bounding box containing the array [minimum latitude, maximum latitude, minimum longitude, maximum longitude]. |
|**Required**            |True|
|**Type**                |List|
|**Style**               |float pairs|
|**Units or options**    | decimal degree |
|**Example**             |[39.797, 39.813, -119.013, -118.995]|

### cable_owner
|attributeID              |<div align="right">cable_owner <img width=200/> <code>Optional</code> </div>|
|:------------------------|:----------------------------------------------------|
|**Description**         |Proprietary owner of the cable. |
|**Required**            |True|
|**Type**                |String|
|**Style**               |Alphanumeric|
|**Units or options**    | -- |
|**Example**             |CA001|

### cable_installation_date
|attributeID              |<div align="right">cable_installation_date <img width=200/> <code>Optional</code> </div>|
|:------------------------|:----------------------------------------------------|
|**Description**         |Cable installation date in UTC. This may not be known, an optional field. |
|**Required**            |True|
|**Type**                |String|
|**Style**               |ISO formatted date|
|**Units or options**    | na |
|**Example**             | - |

### cable_removal_date
|attributeID              |<div align="right">cable_removal_date <img width=200/> <code>Optional</code> </div>|
|:------------------------|:----------------------------------------------------|
|**Description**         |Cable removal date in UTC. This may not be known, an optional field. |
|**Required**            |True|
|**Type**                |String|
|**Style**               |ISO formatted date|
|**Units or options**    | na |
|**Example**             | - |

### cable_characteristics
|attributeID              |<div align="right">cable_characteristics <img width=200/> <code>Optional</code> </div>|
|:------------------------|:----------------------------------------------------|
|**Description**         |Describes how the fiber is encased in the cable.|
|**Required**            | False|
|**Type**                |String|
|**Style**               |Controlled vocabulary|
|**Units or options**    | [buffered | armored | gel-filled | other] |
|**Example**             | buffered |

### cable_environment
|attributeID              |<div align="right">cable_environment <img width=200/> <code>Optional</code> </div>|
|:------------------------|:----------------------------------------------------|
|**Description**         |Describes the installation environment of cable.|
|**Required**            | False|
|**Type**                |String|
|**Style**               |Controlled vocabulary|
|**Units or options**    | [conduit | trench | outside borehole casing | wireline | other] |
|**Example**             | trench |

### cable_installation_environment
|attributeID              |<div align="right">cable_installation_environment <img width=200/> <code>Optional</code> </div>|
|:------------------------|:----------------------------------------------------|
|**Description**         |Plain language description of how the cable was installed.|
|**Required**            |False|
|**Type**                |String|
|**Style**               |Free form text|
|**Units or options**    | -- |
|**Example**             |na|

### cable_model
|attributeID              |<div align="right">cable_model <img width=200/> <code>Optional</code> </div>|
|:------------------------|:----------------------------------------------------|
|**Description**         |Cable manufacturer model.|
|**Required**            |False|
|**Type**                |String|
|**Style**               |Free form text|
|**Units or options**    | -- |
|**Example**             |na|

### cable_outside_diameter
|attributeID              |<div align="right">cable_outside_diameter <img width=200/> <code>Optional</code> </div>|
|:------------------------|:----------------------------------------------------|
|**Description**         |Cable outside diameter.|
|**Required**            |False|
|**Type**                |Float|
|**Style**               | na |
|**Units or options**    | -- |
|**Example**             | -- |

### cable_outside_diameter_unit
|attributeID              |<div align="right">cable_outside_diameter_unit <img width=200/> <code>Optional</code> </div>|
|:------------------------|:----------------------------------------------------|
|**Description**         |Unit of outside diameter of cable.|
|**Required**            | False|
|**Type**                |String|
|**Style**               |Controlled vocabulary|
|**Units or options**    | millimeter |
|**Example**             | trench |

### comment
|attributeID              |<div align="right">comment <img width=200/> <code>Optional</code> </div>|
|:------------------------|:----------------------------------------------------|
|**Description**         |Additional comments.|
|**Required**            |False|
|**Type**                |String|
|**Style**               |Free form text|
|**Units or options**    | -- |
|**Example**             |na|
