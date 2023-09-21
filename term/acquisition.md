**Acquisition Metadata**
* The Acquisition metadata describes the acquisition parameters set by the user on a particular interrogator. While different interrogator vendors may implement various photonics design and algorithms which are not easily translatable across interrogators, the Acquisition metadata intends to capture the critical acquisition attributes that are commonly required to analyze and interpret the output time series or matrices. These attributes are carefully defined to be standardized across all interrogator systems. While the Acquisition metadata listed below should be self-sufficient for most purposes, the native headers provided by interrogator vendors can be preserved for expert users.

* Required fields *(mark with an asterisk, and indicated in the tables below)*
[acquisition_id*](#acquisition_id) |
[interrogator_id*](#interrogator_id) |
[acquisition_start_time*](#acquisition_start_time) |
[acquisition_end_time*](#acquisition_end_time) |
[acquisition_sample_rate*](#acquisition_sample_rate) |
[acquisition_sample_rate_unit*](#acquisition_sample_rate_unit) |
[gauge_length*](#gauge_length) |
[gauge_length_unit*](#gauge_length_unit) |
[unit_of_measure*](#unit_of_measure) |
[number_of_channels*](#number_of_channels) |
[spatial_sampling_interval*](#spatial_sampling_interval) |
[spatial_sampling_interval_unit*](#spatial_sampling_interval_unit) 

* Optional fields\
[pulse_rate](#pulse_rate) |
[pulse_rate_unit](#pulse_rate_unit) |
[pulse_width](#pulse_width) |
[pulse_width_unit](#pulse_width_unit) |
[comment](#comment)

---

### acquisition_id
|attributeID              |<div align="right">acquisition_id <img width=200/> <code>Required</code> </div>|
|:------------------------|:----------------------------------------------------|
|**Description**         |Unique identifier of the data acquisition, assigned by data provider. Identifier should have a maximum of 8 alphanumeric characters with no special characters (e.g., underscores, period, dash). One identifier per acquisition settings. |
|**Required**            |True|
|**Type**                |String|
|**Style**               |Alphanumeric|
|**Units or options**    | -- |
|**Example**             |A001|

### interrogator_id
|attributeID              |<div align="right">interrogator_id <img width=200/> <code>Required</code> </div>|
|:------------------------|:----------------------------------------------------|
|**Description**         |Unique identifier of the interrogator unit used in this data acquisition. The acquisition_id must nest within this interrogator_id. |
|**Required**            |True|
|**Type**                |String|
|**Style**               |Alphanumeric|
|**Units or options**    | -- |
|**Example**             |IU001|

### acquisition_start_time
|attributeID              |<div align="right">acquisition_start_time <img width=200/> <code>Required</code> </div>|
|:------------------------|:----------------------------------------------------|
|**Description**         |Start time of this data acquisition in UTC.|
|**Required**            |True|
|**Type**                |String|
|**Style**               |ISO formatted datetime|
|**Units or options**    | -- |
|**Example**             |2016-03-11T16:46:18.000Z|

### acquisition_end_time
|attributeID              |<div align="right">acquisition_end_time <img width=200/> <code>Required</code> </div>|
|:------------------------|:----------------------------------------------------|
|**Description**         |End time of this data acquisition in UTC. if data acquisition is still in operation, use a date in the future (e.g. 2999-01-01T00:00:00.000Z).|
|**Required**            |True|
|**Type**                |String|
|**Style**               |ISO formatted datetime|
|**Units or options**    | na |
|**Example**             |2016-03-26T01:01:15.000Z|

### acquisition_sample_rate
|attributeID              |<div align="right">acquisition_sample_rate <img width=200/> <code>Required</code> </div>|
|:------------------------|:----------------------------------------------------|
|**Description**         |The rate at which the interrogator provides output data. |
|**Required**            |True|
|**Type**                |Integer|
|**Style**               |na|
|**Units or options**    |na |
|**Example**             |1000|

### acquisition_sample_rate_unit
|attributeID              |<div align="right">acquisition_sample_rate_unit <img width=200/> <code>Required</code> </div>|
|:------------------------|:----------------------------------------------------|
|**Description**         |Unit of acquisition sample rate. |
|**Required**            |True|
|**Type**                |String|
|**Style**               |Controlled vocabulary|
|**Units or options**    | Hertz |
|**Example**             | Hertz |

### gauge_length
|attributeID              |<div align="right">gauge_length <img width=200/> <code>Required</code> </div>|
|:------------------------|:----------------------------------------------------|
|**Description**         | The length along the fiber between a pair of pulses, determined at experiment setup and used during acquisition. |
|**Required**            | True|
|**Type**                | Float |
|**Style**               | na |
|**Units or options**    | na |
|**Example**             | 10 |

### gauge_length_unit
|attributeID              |<div align="right">gauge_length_unit <img width=200/> <code>Required</code> </div>|
|:------------------------|:----------------------------------------------------|
|**Description**         | Unit of gauge length. |
|**Required**            | True|
|**Type**                | String |
|**Style**               | Controlled vocabulary |
|**Units or options**    | meter |
|**Example**             | meter |

### unit_of_measure
|attributeID              |<div align="right">unit_of_measure <img width=200/> <code>Required</code> </div>|
|:------------------------|:----------------------------------------------------|
|**Description**         | Unit of measure of archived data set. This may be the same unit as the Interrogator Unit of Measure if the data are raw. |
|**Required**            | True|
|**Type**                | String |
|**Style**               | Controlled vocabulary |
|**Units or options**    | [count | strain | strain-rate | velocity] |
|**Example**             | count |

### number_of_channels
|attributeID              |<div align="right">number_of_channels <img width=200/> <code>Required</code> </div>|
|:------------------------|:----------------------------------------------------|
|**Description**         | The total number of sampling points along the fiber as output from the interrogator, referred to as NumberOfLoci in PRODML. |
|**Required**            | True|
|**Type**                | Integer |
|**Style**               | na |
|**Units or options**    | na |
|**Example**             | 8720 |

### spatial_sampling_interval
|attributeID              |<div align="right">spatial_sampling_interval <img width=200/> <code>Required</code> </div>|
|:------------------------|:----------------------------------------------------|
|**Description**         | The channel spacing, or offset, between channels. |
|**Required**            | True|
|**Type**                | Float |
|**Style**               | na |
|**Units or options**    | na |
|**Example**             | 1.000 |

### spatial_sampling_interval_unit
|attributeID              |<div align="right">spatial_sampling_interval_unit <img width=200/> <code>Required</code> </div>|
|:------------------------|:----------------------------------------------------|
|**Description**         | Unit of spatial sampling interval. |
|**Required**            | True|
|**Type**                | String |
|**Style**               | Controlled vocabulary |
|**Units or options**    | meter |
|**Example**             | meter |

### pulse_rate
|attributeID              |<div align="right">pulse_rate <img width=200/> <code>Optional</code> </div>|
|:------------------------|:----------------------------------------------------|
|**Description**         |Rate at which the interrogator unit interrogates the fiber sensor.|
|**Required**            |False|
|**Type**                |Float|
|**Style**               |na|
|**Units or options**    | -- |
|**Example**             | 1000 |

### pulse_rate_unit
|attributeID              |<div align="right">pulse_rate_unit <img width=200/> <code>Optional</code> </div>|
|:------------------------|:----------------------------------------------------|
|**Description**         |Unit of pulse rate.|
|**Required**            |False|
|**Type**                |String|
|**Style**               |Controlled vocabulary|
|**Units or options**    | Hertz |
|**Example**             | Hertz |

### pulse_width
|attributeID              |<div align="right">pulse_width <img width=200/> <code>Optional</code> </div>|
|:------------------------|:----------------------------------------------------|
|**Description**         |Width of the pulse sent down the fiber in unit of time. |
|**Required**            |False|
|**Type**                |Float|
|**Style**               |na|
|**Units or options**    | -- |
|**Example**             | -- |

### pulse_width_unit
|attributeID              |<div align="right">pulse_rate_unit <img width=200/> <code>Optional</code> </div>|
|:------------------------|:----------------------------------------------------|
|**Description**         |Unit of pulse width.|
|**Required**            |False|
|**Type**                |String|
|**Style**               |Controlled vocabulary|
|**Units or options**    | nanoseconds |
|**Example**             | nanoseconds |

### comment
|attributeID              |<div align="right">comment <img width=200/> <code>Optional</code> </div>|
|:------------------------|:----------------------------------------------------|
|**Description**         |Additional comments.|
|**Required**            |False|
|**Type**                |String|
|**Style**               |Free form text|
|**Units or options**    | -- |
|**Example**             |na|
