**Cable and Fiber Metadata**:      
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

*Required fields are marked with an asterisk, and indicated in detailed tables below.


---

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
