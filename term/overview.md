**Overview Metadata**
* The Overview metadata gives a high-level overview of the DAS deployment and describes the geographic location of the installation, dates of the project, and information on the data provider.

* Required fields *(mark with an asterisk, and indicated in the tables below)*\
[network_code*](#network_code) |
[location*](#location) |
[country*](#country) |
[principal_investigator_name*](#principal_investigator_name) |
[principal_investigator_email*](#principal_investigator_email) |
[principal_investigator_address*](#principal_investigator_address) |
[point_of_contact*](#point_of_contact) |
[point_of_contact_email*](#point_of_contact_email) |
[point_of_contact_address*](#point_of_contact_address) |
[start_date*](#start_date) |
[end_date*](#end_date)


* Optional fields\
[funding_agency](#funding_agency) |
[project_number](#project_number) |
[digital_object_identifier](#digital_object_identifier) |
[purpose_of_data_collection](#purpose_of_data_collection) |
[comment](#comment)


---

### network_code
|attributeID              |<div align="right">network_code <img width=200/> <code>Required</code> </div>|
|:------------------------|:----------------------------------------------------|
|**Description**         |Unique network name for the installation with a maximum of 8 alphanumeric characters with no special characters (e.g., underscores, period, dash). |
|**Required**            |True|
|**Type**                |String|
|**Style**               |Alphanumeric|
|**Units or options**    | -- |
|**Example**             |NVPORO|

### location
|attributeID              |<div align="right">location <img width=200/> <code>Required</code> </div>|
|:------------------------|:----------------------------------------------------|
|**Description**         |Name of the geographic location of the installation. |
|**Required**            |True|
|**Type**                |String|
|**Style**               |Free form text|
|**Units or options**    | -- |
|**Example**             |Brady's Hot Springs, Nevada|

### country
|attributeID              |<div align="right">country <img width=200/> <code>Required</code> </div>|
|:------------------------|:----------------------------------------------------|
|**Description**         |Country where the installation is located. Use ISO 3166-1 alpha-3 three-letter country code. |
|**Required**            |True|
|**Type**                |String|
|**Style**               |Free form text|
|**Units or options**    | -- |
|**Example**             |USA|

### principal_investigator_name
|attributeID              |<div align="right">principal_investigator_name <img width=200/> <code>Required</code> </div>|
|:------------------------|:----------------------------------------------------|
|**Description**         |Name of principal investigator for the installation.|
|**Required**            |True|
|**Type**                |String|
|**Style**               |Free form text|
|**Units or options**    | -- |
|**Example**             |USA|


### principal_investigator_email
|attributeID              |<div align="right">principal_investigator_email <img width=200/> <code>Required</code> </div>|
|:------------------------|:----------------------------------------------------|
|**Description**         |Email address of principal investigator.|
|**Required**            |True|
|**Type**                |String|
|**Style**               |Email address|
|**Units or options**    | -- |
|**Example**             | -- |

### principal_investigator_address
|attributeID              |<div align="right">principal_investigator_address <img width=200/> <code>Required</code> </div>|
|:------------------------|:----------------------------------------------------|
|**Description**         |Physical address and institution of principal investigator.|
|**Required**            |True|
|**Type**                |String|
|**Style**               |Free form text|
|**Units or options**    | -- |
|**Example**             |University of Wisconsin|

### point_of_contact
|attributeID              |<div align="right">point_of_contact <img width=200/> <code>Required</code> </div>|
|:------------------------|:----------------------------------------------------|
|**Description**         |Point of contact for the metadata.|
|**Required**            |True|
|**Type**                |String|
|**Style**               |Free form text|
|**Units or options**    | -- |
|**Example**             | -- |

### point_of_contact_email
|attributeID              |<div align="right">point_of_contact_email <img width=200/> <code>Required</code> </div>|
|:------------------------|:----------------------------------------------------|
|**Description**         |Email address of point of contact.|
|**Required**            |True|
|**Type**                |String|
|**Style**               |Email address|
|**Units or options**    | -- |
|**Example**             | -- |

### point_of_contact_address
|attributeID              |<div align="right">point_of_contact_address <img width=200/> <code>Required</code> </div>|
|:------------------------|:----------------------------------------------------|
|**Description**         |Physical address and institution of point of contact.|
|**Required**            |True|
|**Type**                |String|
|**Style**               |Free form text|
|**Units or options**    | -- |
|**Example**             |University of Wisconsin|

### start_date
|attributeID              |<div align="right">start_date <img width=200/> <code>Required</code> </div>|
|:------------------------|:----------------------------------------------------|
|**Description**         |Start date of data collection at the installation in UTC.|
|**Required**            |True|
|**Type**                |String|
|**Style**               |ISO formatted date|
|**Units or options**    | -- |
|**Example**             |2016-03-11|

### end_date
|attributeID              |<div align="right">end_date <img width=200/> <code>Required</code> </div>|
|:------------------------|:----------------------------------------------------|
|**Description**         |End date of data collection at the installation in UTC. If installation is still in operation, use a future date (e.g. 2999-01-01).|
|**Required**            |True|
|**Type**                |String|
|**Style**               |ISO formatted date|
|**Units or options**    | -- |
|**Example**             |2016-03-26|


### funding_agency
|attributeID              |<div align="right">funding_agency <img width=200/> <code>Optional</code> </div>|
|:------------------------|:----------------------------------------------------|
|**Description**         |Name(s) of agency that funded the experiment.|
|**Required**            |False|
|**Type**                |String|
|**Style**               |Free form text|
|**Units or options**    | -- |
|**Example**             |U.S. DOE Geothermal Technology Office|

### project_number
|attributeID              |<div align="right">project_number <img width=200/> <code>Optional</code> </div>|
|:------------------------|:----------------------------------------------------|
|**Description**         |Funding project number. Should be supplied if a number has been assigned by funding agency(s).|
|**Required**            |False|
|**Type**                |String|
|**Style**               |Free form text|
|**Units or options**    | -- |
|**Example**             |DOE CN: EE0006760|

### digital_object_identifier
|attributeID              |<div align="right">digital_object_identifier <img width=200/> <code>Optional</code> </div>|
|:------------------------|:----------------------------------------------------|
|**Description**         |Digital Object Identifier that uniquely identifies the metadata, this identifier may only become available following archiving.|
|**Required**            |False|
|**Type**                |String|
|**Style**               |URL|
|**Units or options**    | -- |
|**Example**             |https://doi.org/10.15121/1778858|

### purpose_of_data_collection
|attributeID              |<div align="right">purpose_of_data_collection <img width=200/> <code>Optional</code> </div>|
|:------------------------|:----------------------------------------------------|
|**Description**         |Brief explanation of the purpose of experiment.|
|**Required**            |False|
|**Type**                |String|
|**Style**               |Free form text|
|**Units or options**    | -- |
|**Example**             |Monitor geothermal field|

### comment
|attributeID              |<div align="right">comment <img width=200/> <code>Optional</code> </div>|
|:------------------------|:----------------------------------------------------|
|**Description**         |Additional comments.|
|**Required**            |False|
|**Type**                |String|
|**Style**               |Free form text|
|**Units or options**    | -- |
|**Example**             | -- |
