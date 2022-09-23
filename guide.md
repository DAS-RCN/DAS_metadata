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
[Cable model](#cable-model) |
[Cable diameter](#cable-diameter) |
[Cable coordinates*](#cable-coordinates) |
[Cable connector coordinates](#cable-connector-coordinates) |
[Fiber mode](#fiber-mode) |
[Fiber refraction index](#fiber-refraction-index) |
[Attenuation](#attenuation) |
[Fiber geometry](#fiber-geometry) |
[Winding angle](#winding-angle) |
[Fiber start location](#fiber-start-location) |
[Fiber end location](#fiber-end-location) |
[Fiber length](#fiber-length) |
[Comment](#comment) |

**[Interrogator](#interrogator-metadata)**:      
[Interrogator ID*](#interrogator-ID) |
[Manufacturer*](#manufacturer) |
[Model*](#model) |
[Unit of measure*](#unit-of-measure) |

**[Acquisition Metadata](#acquisition-metadata)**:      
[Acquisition ID*](#acquisition-ID) |
[Acquisition start time*](#acquisition-start-time) |
[Acquisition end time*](#acquisition-end-time) |
[Acquisition sample rate*](#acquisition-sample-rate) |
[Pulse repetition rate](#pulse-repetition-rate) |
[Interrogator rate](#interrogator-rate) |
[Pulse width](#pulse-width) |
[Gauge length*](#gauge-length) |
[Number of channels*](#number-of-channels) |
[Channel spacing*](#channel-spacing) |
[Archived sample rate*](#archived-sample-rate) |
[Unit of measure*](#unit-of-measure) |
[Decimation*](#decimation) |
[Filtering*](#filtering) |
[Comment](#comment) |

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

---
## Cable and Fiber Metadata

### Cable fiber ID
|AttributeID              |<div align="right">cable_fiber_id <img width=200/> <code>Required</code> </div>| 
|:------------------------|:----------------------------------------------------|
|**Definition**           |A term that identifies the fiber used within an experiment defined by the researcher|
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
|**Format**               |Controlled vocabulary|
|**Options**              |[buffered, armored, gel-filled]|
|**Additional Instructions**| -- 
|**Examples**             |gel-filled|

### Cable environment
|AttributeID              |<div align="right">cable_environment <img width=200/> <code>Optional</code> </div>| 
|:------------------------|:----------------------------------------------------|
|**Definition**           |describes the installation environment|
|**Type**                 |String|
|**Format**               |Controlled vocabulary|
|**Options**              |[Conduit, trench, outside borehole casing, wireline]|
|**Additional Instructions**| -- 
|**Examples**             |outside borehole casing|

### Cable model
|AttributeID              |<div align="right">cable_model <img width=200/> <code>Optional</code> </div>| 
|:------------------------|:----------------------------------------------------|
|**Definition**           |Cable manufacturer model|
|**Type**                 |String|
|**Format**               |Alpha Numeric|
|**Additional Instructions**| -- 
|**Examples**             |MD1234|

### Cable diameter
|AttributeID              |<div align="right">cable_diameter <img width=200/> <code>Optional</code> </div>| 
|:------------------------|:----------------------------------------------------|
|**Definition**           |Cable diameter|
|**Type**                 |Float|
|**Unit**                 |meter|
|**Additional Instructions**| -- 
|**Examples**             |0.01|

### Cable coordinates
|AttributeID              |<div align="right">cable_coordinates <img width=200/> <code>Optional</code> </div>| 
|:------------------------|:----------------------------------------------------|
|**Definition**           |List of cable coordinates. List should include a descriptor that indicates how positions were determined and a version number. |
|**Type**                 |Dictionary|
|**Unit**                 |WGS84 or meters|
|**Additional Instructions**| -- 
|**Examples**             | |

### Cable connector coordinates
|AttributeID              |<div align="right">cable_connector_coordinates <img width=200/> <code>Optional</code> </div>| 
|:------------------------|:----------------------------------------------------|
|**Definition**           |List of coordinates of connectors (if any) along a cable. List should include descriptors for how positions were determined. |
|**Type**                 |Dictionary|
|**Unit**                 |WGS84 or meters|
|**Additional Instructions**| -- 
|**Examples**             | |

### Fiber mode
|AttributeID              |<div align="right">fiber_mode <img width=200/> <code>Optional</code> </div>| 
|:------------------------|:----------------------------------------------------|
|**Definition**           |Fiber mode|
|**Type**                 |String|
|**Format**               |Controlled vocabulary|
|**Options**              |[single, multimode]|
|**Additional Instructions**| -- 
|**Examples**             |multimode|

### Fiber refraction index
|AttributeID              |<div align="right">fiber_refraction_index <img width=200/> <code>Required</code> </div>| 
|:------------------------|:----------------------------------------------------|
|**Definition**           |Fiber refraction index|
|**Type**                 |Float|
|**Unit**                 |None|
|**Additional Instructions**| -- 
|**Examples**             |0.2|

### Attenuation
|AttributeID              |<div align="right">attenuation <img width=200/> <code>Optional</code> </div>| 
|:------------------------|:----------------------------------------------------|
|**Definition**           |Signal loss along fiber|
|**Type**                 |Float|
|**Unit**                 |dB/km|
|**Additional Instructions**| -- 
|**Examples**             | |

### Fiber geometry
|AttributeID              |<div align="right">fiber_geometry <img width=200/> <code>Optional</code> </div>| 
|:------------------------|:----------------------------------------------------|
|**Definition**           |Geometry of cable|
|**Type**                 |String|
|**Format**               |Controlled vocabulary|
|**Options**              |[linear , helical]|
|**Additional Instructions**| -- 
|**Examples**             |linear|

### Winding angle
|AttributeID              |<div align="right">winding_angle <img width=200/> <code>Required</code> </div>| 
|:------------------------|:----------------------------------------------------|
|**Definition**           |Winding angle with respect to cable axis|
|**Type**                 |Float|
|**Unit**                 |degrees|
|**Additional Instructions**| -- 
|**Examples**             |20|

### Fiber start location
|AttributeID              |<div align="right">fiber_start_location <img width=200/> <code>Required</code> </div>| 
|:------------------------|:----------------------------------------------------|
|**Definition**           |start location wrt the IU (if different from cable)|
|**Type**                 |Float|
|**Unit**                 |km|
|**Additional Instructions**| -- 
|**Examples**             |5|

### Fiber end location
|AttributeID              |<div align="right">fiber_end_location <img width=200/> <code>Required</code> </div>| 
|:------------------------|:----------------------------------------------------|
|**Definition**           |end location wrt the IU (if different from cable)|
|**Type**                 |Float|
|**Unit**                 |km|
|**Additional Instructions**| -- 
|**Examples**             |10|

### Fiber length
|AttributeID              |<div align="right">fiber_length <img width=200/> <code>Required</code> </div>| 
|:------------------------|:----------------------------------------------------|
|**Definition**           |.  |
|**Type**                 |Float|
|**Unit**                 |km|
|**Additional Instructions**| -- 
|**Examples**             |8.5|

### Comment
|AttributeID              |<div align="right">comment <img width=200/> <code>Optional</code> </div>| 
|:------------------------|:----------------------------------------------------|
|**Definition**           |Add additional comment|
|**Type**                 |String|
|**Format**               |Free form|
|**Additional Instructions**| -- 
|**Examples**             |--|

---
## Interrogator Metadata

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

---
## Acquistion Metadata

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
