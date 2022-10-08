**Acquisition Metadata**
* Contains information on data collection, sample rate, pulse length, gauge length, channel spacing, and signal-processing steps.

* Required fields *(mark with an asterisk, and indicated in the tables below)*  
[Acquisition ID*](#acquisition-ID) |
[Acquisition start time*](#acquisition-start-time) |
[Acquisition end time*](#acquisition-end-time) |
[Acquisition sample rate*](#acquisition-sample-rate) |
[Gauge length*](#gauge-length) |
[Number of channels*](#number-of-channels) |
[Channel spacing*](#channel-spacing) |
[Archived sample rate*](#archived-sample-rate) |
[Unit of measure*](#unit-of-measure) |
[Decimation*](#decimation) |
[Filtering*](#filtering) |

* Optional fields
[Pulse repetition rate](#pulse-repetition-rate) |
[Interrogator rate](#interrogator-rate) |
[Pulse width](#pulse-width) |
[Comment](#comment) |

---

### Acquisition ID
|AttributeID              |<div align="right">acquisition_id <img width=200/> <code>Required</code> </div>| 
|:------------------------|:----------------------------------------------------|
|**Definition**           |User defined, one identifier per acquisition period|
|**Type**                 |String|
|**Format**               |Alpha Numeric|
|**Default**              |1|
|**Additional Instructions**| -- 
|**Examples**             |1A|

### Acquisition start time
|AttributeID              |<div align="right">acquisition_start_time <img width=200/> <code>Required</code> </div>| 
|:------------------------|:----------------------------------------------------|
|**Definition**           |Start date of data collection|
|**Type**                 |String|
|**Format**               |ISO formatted date-time|
|**Unit**                 |UTC|
|**Additional Instructions**| -- 
|**Examples**             |yyyy-mm-ddTHH:mm:ss|

### Acquisition end time
|AttributeID              |<div align="right">acquisition_end_time <img width=200/> <code>Required</code> </div>| 
|:------------------------|:----------------------------------------------------|
|**Definition**           |End date of data collection|
|**Type**                 |String|
|**Format**               |ISO formatted date-time|
|**Unit**                 |UTC|
|**Additional Instructions**| -- 
|**Examples**             |yyyy-mm-ddTHH:mm:ss|

### Acquisition sample rate
|AttributeID              |<div align="right">acquisition_sample_rate <img width=200/> <code>Required</code> </div>| 
|:------------------------|:----------------------------------------------------|
|**Definition**           |The rate at which the interrogator provides output data|
|**Type**                 |Integer|
|**Unit**                 |Hz (1/s)|
|**Additional Instructions**| -- 
|**Examples**             |500|

### Pulse repetition rate
|AttributeID              |<div align="right">pulse_repetition_rate <img width=200/> <code>Optional</code> </div>| 
|:------------------------|:----------------------------------------------------|
|**Definition**           |Number of pulses per second|
|**Type**                 |Integer|
|**Unit**                 |Hz (1/s)|
|**Additional Instructions**| -- 
|**Examples**             |1000|

### Interrogator rate
|AttributeID              |<div align="right">interrogator_rate <img width=200/> <code>Optional</code> </div>| 
|:------------------------|:----------------------------------------------------|
|**Definition**           |Rate at which the Interrogator Unit interrogates the fiber |
|**Type**                 |Integer|
|**Unit**                 |Hz (1/s)|
|**Additional Instructions**| -- 
|**Examples**             |1000|

### Pulse width
|AttributeID              |<div align="right">pulse_width <img width=200/> <code>Optional</code> </div>| 
|:------------------------|:----------------------------------------------------|
|**Definition**           |The length in time of the width of the pulse, or burst of light, sent down the fiber |
|**Type**                 |Float|
|**Unit**                 |seconds|
|**Additional Instructions**| -- 
|**Examples**             |4x10^-8|

### Gauge length
|AttributeID              |<div align="right">gauge_length <img width=200/> <code>Required</code> </div>| 
|:------------------------|:----------------------------------------------------|
|**Definition**           |The length along the fiber between a pair of pulses, determined at experiment setup  |
|**Type**                 |Float|
|**Unit**                 |meter|
|**Additional Instructions**| -- 
|**Examples**             |10|

### Number of channels
|AttributeID              |<div align="right">number_of_channels <img width=200/> <code>Required</code> </div>| 
|:------------------------|:----------------------------------------------------|
|**Definition**           |Total number of channels in archived data set  |
|**Type**                 |Integer|
|**Additional Instructions**| -- 
|**Examples**             |1000|

### Channel spacing
|AttributeID              |<div align="right">channel_spacing <img width=200/> <code>Required</code> </div>| 
|:------------------------|:----------------------------------------------------|
|**Definition**           |Spacing between channels  |
|**Type**                 |Float|
|**Unit**                 |meter|
|**Additional Instructions**| -- 
|**Examples**             |2|

### Archived sample rate
|AttributeID              |<div align="right">archived_sample_rate <img width=200/> <code>Required</code> </div>| 
|:------------------------|:----------------------------------------------------|
|**Definition**           |Sample rate of archived data set (this will equal the acquisition sample rate if there is no decimation)|
|**Type**                 |Integer|
|**Unit**                 |Hz (1/s)|
|**Additional Instructions**| -- 
|**Examples**             |1000|

### Unit of measure
|AttributeID              |<div align="right">unit_of_measure <img width=200/> <code>Required</code> </div>| 
|:------------------------|:----------------------------------------------------|
|**Definition**           |Interrogators natural unit of measure|
|**Type**                 |String|
|**Format**               |Controlled vocabulary|
|**Options**              |[natural units, strain, strain-rate, velocity]|
|**Additional Instructions**| -- 
|**Examples**             |strain-rate|

### Decimation
|AttributeID              |<div align="right">decimation <img width=200/> <code>Required</code> </div>| 
|:------------------------|:----------------------------------------------------|
|**Definition**           |If no decimation applied the default = 0|
|**Type**                 |Integer|
|**Default**              |0|
|**Additional Instructions**| -- 
|**Examples**             |0|

### Filtering
|AttributeID              |<div align="right">filtering <img width=200/> <code>Required</code> </div>| 
|:------------------------|:----------------------------------------------------|
|**Definition**           |Filtering process applied to time series |
|**Type**                 |String|
|**Format**               |Controlled vocabulary|
|**Options**              |[high pass, band pass, low pass]|
|**Unit**                 |Filter Type/frequency band|
|**Additional Instructions**| -- 
|**Examples**             |Bandpass 1 - 100 Hz|

### Comment
|AttributeID              |<div align="right">comment <img width=200/> <code>Optional</code> </div>| 
|:------------------------|:----------------------------------------------------|
|**Definition**           |Add additional comment|
|**Type**                 |String|
|**Format**               |Free form|
|**Additional Instructions**| -- 
|**Examples**             |--|
