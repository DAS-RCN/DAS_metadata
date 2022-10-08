**Channel Metadata**
* Describes each individual channel along the fiber, e.g., position, pulse direction, and location method. One possibility here is to have a pointer to a file(s) with a known format (e.g. kml, csv) rather than repeat all information.

* Required fields *(mark with an asterisk, and indicated in the tables below)*  
[Name of asssociated file*](#name-of-associated-file) |
[File format of asssociated file*](#file-format-of-associated-file) |
[Generation date*](#generation-date) |
[Channel ID*](#channel-id) |
[Reference frame*](#reference-frame) |
[Location method*](#location-method) |
[Direction of laser pulse*](#direction-of-laser-pulse) 

**[Coordinate file](#coordinate-file)**: 
[Channel ID*](#channel-id) |
[Distance along fiber*](#distance-along-fiber) |
[Y coordinate*](#y-coordinate) |
[X coordinate*](#x-coordinate) |
[Depth*](#depth) 

* Optional fields
[Y coordinate error](#y-coordinate-error) |
[X coordinate error](#x-coordinate-error) |
[Elevation](#elevation) |
[Elevation error](#elevation-error) |
[Depth error](#depth-error) |
[Strike](#strike) |
[Strike error](#strike-error) |
[Dip](#dip) |
[Dip error](#dip-error) |
[Comment](#comment) 

---

### Name of associated file
|AttributeID              |<div align="right">channel_file <img width=200/> <code>Required</code> </div>| 
|:------------------------|:----------------------------------------------------|
|**Definition**           |Name of an file attached to data set|
|**Type**                 |String|
|**Format**               |Free form|
|**Additional Instructions**| -- 
|**Examples**             |coordinates.txt|

### File format of associated file
|AttributeID              |<div align="right">channel_file_format <img width=200/> <code>Required</code> </div>| 
|:------------------------|:----------------------------------------------------|
|**Definition**           |Format of associated file |
|**Type**                 |String|
|**Format**               |Controlled vocabulary|
|**Options**              |[KML, CSV, txt, XML, pdf]|
|**Additional Instructions**| -- 
|**Examples**             |CSV|

### Generation date
|AttributeID              |<div align="right">generation_date <img width=200/> <code>Required</code> </div>| 
|:------------------------|:----------------------------------------------------|
|**Definition**           |Date co-ordinates were generated|
|**Type**                 |String|
|**Format**               |ISO formatted date-time|
|**Unit**                 |UTC|
|**Additional Instructions**| -- 
|**Examples**             |2022-06-24|

### Channel ID
|AttributeID              |<div align="right">channel_id <img width=200/> <code>Required</code> </div>| 
|:------------------------|:----------------------------------------------------|
|**Definition**           |Uniquely identify channel|
|**Type**                 |Integer|
|**Additional Instructions**| -- 
|**Examples**             |100|

### Reference frame
|AttributeID              |<div align="right">reference_frame <img width=200/> <code>Required</code> </div>| 
|:------------------------|:----------------------------------------------------|
|**Definition**           |Geographic_reference_frame, or coordinate system |
|**Type**                 |String|
|**Format**               |Controlled vocabulary|
|**Options**              |[wgs84, UTM, nominal]|
|**Additional Instructions**| -- 
|**Examples**             |wgs84|

### Location method
|AttributeID              |<div align="right">reference_frame <img width=200/> <code>Required</code> </div>| 
|:------------------------|:----------------------------------------------------|
|**Definition**           |Example: Tap tests, GPS, survey |
|**Type**                 |Text|
|**Additional Instructions**| -- 
|**Examples**             |None|

### Direction of laser pulse
|AttributeID              |<div align="right">reference_frame <img width=200/> <code>Optional</code> </div>| 
|:------------------------|:----------------------------------------------------|
|**Definition**           |Increasing trace number |
|**Type**                 |Float|
|**Unit**                 |degrees|
|**Additional Instructions**| -- 
|**Examples**             |None|

### Comment
|AttributeID              |<div align="right">comment <img width=200/> <code>Optional</code> </div>| 
|:------------------------|:----------------------------------------------------|
|**Definition**           |Add additional comment|
|**Type**                 |String|
|**Format**               |Free form|
|**Additional Instructions**| -- 
|**Examples**             |--|

---
## Coordinate file

### Channel ID
|AttributeID              |<div align="right">channel_ID <img width=200/> <code>Required</code> </div>| 
|:------------------------|:----------------------------------------------------|
|**Definition**           |Uniquely identify channel |
|**Type**                 |Integer|
|**Additional Instructions**| -- 
|**Examples**             |None|

### Distance along fiber
|AttributeID              |<div align="right">distance_along_fiber <img width=200/> <code>Required</code> </div>| 
|:------------------------|:----------------------------------------------------|
|**Definition**           |Distance along fiber between the interrogator and channel. |
|**Type**                 |Float|
|**Unit**                 |km|
|**Additional Instructions**| -- 
|**Examples**             |None|

### Y Coordinate
|AttributeID              |<div align="right">y_coordinate <img width=200/> <code>Required</code> </div>| 
|:------------------------|:----------------------------------------------------|
|**Definition**           |Y position of channel within the defined reference frame |
|**Type**                 |Float|
|**Additional Instructions**| -- 
|**Examples**             |None|

### Y Coordinate Error
|AttributeID              |<div align="right">y_coordinate_error <img width=200/> <code>Optional</code> </div>| 
|:------------------------|:----------------------------------------------------|
|**Definition**           |Uncertainty in Y location |
|**Type**                 |Float|
|**Additional Instructions**| -- 
|**Examples**             |None|

### X Coordinate
|AttributeID              |<div align="right">x_coordinate <img width=200/> <code>Required</code> </div>| 
|:------------------------|:----------------------------------------------------|
|**Definition**           |X position of channel within the defined reference frame |
|**Type**                 |Float|
|**Additional Instructions**| -- 
|**Examples**             |None|

### X Coordinate Error
|AttributeID              |<div align="right">x_coordinate_error <img width=200/> <code>Optional</code> </div>| 
|:------------------------|:----------------------------------------------------|
|**Definition**           |Uncertainty in X location |
|**Type**                 |Float|
|**Additional Instructions**| -- 
|**Examples**             |None|

### Elevation
|AttributeID              |<div align="right">elevation <img width=200/> <code>Optional</code> </div>| 
|:------------------------|:----------------------------------------------------|
|**Definition**           |Height above Sea level |
|**Unit**                 |km|
|**Type**                 |Float|
|**Additional Instructions**| -- 
|**Examples**             |None|

### Elevation error
|AttributeID              |<div align="right">elevation_error <img width=200/> <code>Optional</code> </div>| 
|:------------------------|:----------------------------------------------------|
|**Definition**           |Uncertainty in elevation |
|**Unit**                 |km|
|**Type**                 |Float|
|**Additional Instructions**| -- 
|**Examples**             |None|

### Depth
|AttributeID              |<div align="right">depth <img width=200/> <code>Required</code> </div>| 
|:------------------------|:----------------------------------------------------|
|**Definition**           |Depth (positive for depth below surface) |
|**Unit**                 |km|
|**Type**                 |Float|
|**Additional Instructions**| -- 
|**Examples**             |None|

### Depth error
|AttributeID              |<div align="right">depth_error <img width=200/> <code>Optional</code> </div>| 
|:------------------------|:----------------------------------------------------|
|**Definition**           |Uncertainty in elevation, depth below surface is positive?? |
|**Unit**                 |km|
|**Type**                 |Float|
|**Additional Instructions**| -- 
|**Examples**             |None|

### Strike
|AttributeID              |<div align="right">strike <img width=200/> <code>Optional</code> </div>| 
|:------------------------|:----------------------------------------------------|
|**Definition**           |Strike of channel, degrees clockwise of east positive |
|**Unit**                 |degree|
|**Type**                 |Float|
|**Additional Instructions**| -- 
|**Examples**             |None|

### Strike error
|AttributeID              |<div align="right">strike_error <img width=200/> <code>Optional</code> </div>| 
|:------------------------|:----------------------------------------------------|
|**Definition**           |uncertainty in strike|
|**Unit**                 |degree|
|**Type**                 |Float|
|**Additional Instructions**| -- 
|**Examples**             |None|

### Dip
|AttributeID              |<div align="right">dip <img width=200/> <code>Optional</code> </div>| 
|:------------------------|:----------------------------------------------------|
|**Definition**           |Dip of channel |
|**Unit**                 |degree|
|**Type**                 |Float|
|**Additional Instructions**| -- 
|**Examples**             |None|

### Dip error
|AttributeID              |<div align="right">dip_error <img width=200/> <code>Optional</code> </div>| 
|:------------------------|:----------------------------------------------------|
|**Definition**           |Uncertainty in dip|
|**Unit**                 |degree|
|**Type**                 |Float|
|**Additional Instructions**| -- 
|**Examples**             |None|

