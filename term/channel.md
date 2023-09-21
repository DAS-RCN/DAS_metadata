**Channel Metadata**
* Nested under the Channel Group metadata, the individual Channel metadata consists of properties that are unique to each channel, including a unique identifier, coordinates, and for borehole cable, optional strike and dip. Note that the total amount of individual Channel metadata may be equal or less than the number_of_channels attribute specified under Acquisition metadata as only a subset of the channels may be included in the data. This is to accommodate cases where channels cannot be located or omitted due to various reasons.

* Required fields *(mark with an asterisk, and indicated in the tables below)*\
[channel_id*](#channel_id) |
[channel_group_id*](#channel_group_id) |
[distance_along_fiber*](#distance_along_fiber) |
[x_coordinate*](#x_coordinate) |
[y_coordinate*](#y_coordinate) 

* Optional fields\
[elevation_above_sea_level](#elevation_above_sea_level) |
[depth_below_surface](#depth_below_surface) |
[strike](#strike) |
[dip](#dip) 

---

### channel_id
|attributeID              |<div align="right">channel_id <img width=200/> <code>Required</code> </div>|
|:------------------------|:----------------------------------------------------|
|**Description**         |Unique identifier of the individual channel, with a maximum of 8 alphanumeric characters with no special characters (e.g., underscores, period, dash). |
|**Required**            |True|
|**Type**                |String|
|**Style**               |Alphanumeric|
|**Units or options**    | -- |
|**Example**             | 431 |

### channel_group_id
|attributeID              |<div align="right">channel_group_id <img width=200/> <code>Required</code> </div>|
|:------------------------|:----------------------------------------------------|
|**Description**         |Unique identifier of the channel group. |
|**Required**            |True|
|**Type**                |String|
|**Style**               |Alphanumeric|
|**Units or options**    | -- |
|**Example**             | CG001 |

### distance_along_fiber
|attributeID              |<div align="right">distance_along_fiber <img width=200/> <code>Required</code> </div>|
|:------------------------|:----------------------------------------------------|
|**Description**         |Distance along fiber between the interrogator and channel. Zero meter at the connector to the interrogator; negative distances for fiber section inside the interrogator.|
|**Required**            |True|
|**Type**                |Float|
|**Style**               |na|
|**Units or options**    | - |
|**Example**             | na |

### x_coordinate
|attributeID              |<div align="right">x_coordinate <img width=200/> <code>Required</code> </div>|
|:------------------------|:----------------------------------------------------|
|**Description**         |x-coordinate (UTM-x or longitude) of the channel.|
|**Required**            |True|
|**Type**                |Float|
|**Style**               |na|
|**Units or options**    | - |
|**Example**             | 328050.69 |

### y_coordinate
|attributeID              |<div align="right">y_coordinate <img width=200/> <code>Required</code> </div>|
|:------------------------|:----------------------------------------------------|
|**Description**         |y-coordinate (UTM-y or latitude)  of the channel.|
|**Required**            |True|
|**Type**                |Float|
|**Style**               |na|
|**Units or options**    | - |
|**Example**             | 4407542.05 |

### elevation_above_sea_level
|attributeID              |<div align="right">elevation_above_sea_level <img width=200/> <code>Optional</code> </div>|
|:------------------------|:----------------------------------------------------|
|**Description**         |Elevation or height above sea level.|
|**Required**            |False|
|**Type**                |Float|
|**Style**               |na|
|**Units or options**    | - |
|**Example**             | 1231.546 |

### depth_below_surface
|attributeID              |<div align="right">depth_below_surface <img width=200/> <code>Optional</code> </div>|
|:------------------------|:----------------------------------------------------|
|**Description**         |Depth below surface (downwards positive).|
|**Required**            |False|
|**Type**                |Float|
|**Style**               |na|
|**Units or options**    | - |
|**Example**             | - |

### strike
|attributeID              |<div align="right">strike <img width=200/> <code>Optional</code> </div>|
|:------------------------|:----------------------------------------------------|
|**Description**         |Strike of individual channel.|
|**Required**            |False|
|**Type**                |Float|
|**Style**               |na|
|**Units or options**    | - |
|**Example**             | - |

### dip
|attributeID              |<div align="right">dip <img width=200/> <code>Optional</code> </div>|
|:------------------------|:----------------------------------------------------|
|**Description**         |Dip of individual channel.|
|**Required**            |False|
|**Type**                |Float|
|**Style**               |na|
|**Units or options**    | - |
|**Example**             | - |
