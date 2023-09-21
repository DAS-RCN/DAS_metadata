  **Channel Group Metadata**
* The Channel Group metadata describes the properties that are common to all the channels nested under the Interrogator and Acquisition metadata blocks. Having a group-level metadata removes the repetition of common attributes in the individual Channel metadata. This design allows multiple channel groups to exist under the same interrogator and data acquisition settings. The unique identifiers for the interrogator, acquisition, cable and fiber are recorded as well in this metadata block to allows mapping between the interrogator, acquisition, and fiber that were used for this set of coordinates during a particular data collection.

* Required fields *(mark with an asterisk, and indicated in the tables below)*
[channel_group_id*](#channel_group_id) |
[interrogator_id*](#interrogator_id) |
[acquisition_id*](#acquisition_id) |
[cable_id*](#cable_id) |
[fiber_id*](#fiber_id) |
[coordinate_generation_date*](#coordinate_generation_date) |
[coordinate_system*](#coordinate_system) |
[reference_frame*](#reference_frame) |
[location_method*](#location_method) |
[distance_along_fiber_unit*](#distance_along_fiber_unit) |
[x_coordinate_unit*](#x_coordinate_unit) |
[y_coordinate_unit*](#y_coordinate_unit) 

* Optional fields\
[uncertainty_in_x_coordinate](#uncertainty_in_x_coordinate) |
[uncertainty_in_x_coordinate_unit](#uncertainty_in_x_coordinate_unit) |
[uncertainty_in_y_coordinate](#uncertainty_in_y_coordinate) |
[uncertainty_in_y_coordinate_unit](#uncertainty_in_y_coordinate_unit) |
[elevation_above_sea_level_unit](#elevation_above_sea_level_unit) |
[uncertainty_in_elevation](#uncertainty_in_elevation) |
[uncertainty_in_elevation_unit](#uncertainty_in_elevation_unit) |
[depth_below_surface_unit](#depth_below_surface_unit) |
[uncertainty_in_depth](#uncertainty_in_depth) |
[uncertainty_in_depth_unit](#uncertainty_in_depth_unit) |
[strike_unit](#strike_unit) |
[uncertainty_in_strike](#uncertainty_in_strike) |
[uncertainty_in_strike_unit](#uncertainty_in_strike_unit) |
[dip_unit](#dip_unit) |
[uncertainty_in_dip](#uncertainty_in_dip) |
[uncertainty_in_dip_unit](#uncertainty_in_dip_unit) |
[first_usable_channel_id](#first_usable_channel_id) |
[last_usable_channel_id](#last_usable_channel_id) |
[comment](#comment)

---

### channel_group_id
|attributeID              |<div align="right">channel_group_id <img width=200/> <code>Required</code> </div>|
|:------------------------|:----------------------------------------------------|
|**Description**         |Unique identifier of the channel group. Identifier should have a maximum of 8 alphanumeric characters with no special characters (e.g., underscores, period, dash). |
|**Required**            |True|
|**Type**                |String|
|**Style**               |Alphanumeric|
|**Units or options**    | -- |
|**Example**             |CG001|

### interrogator_id
|attributeID              |<div align="right">interrogator_id <img width=200/> <code>Required</code> </div>|
|:------------------------|:----------------------------------------------------|
|**Description**         |Unique identifier of interrogator used corresponding to this channel group. |
|**Required**            |True|
|**Type**                |String|
|**Style**               |Alphanumeric|
|**Units or options**    | -- |
|**Example**             |IU001|

### acquisition_id
|attributeID              |<div align="right">acquisition_id <img width=200/> <code>Required</code> </div>|
|:------------------------|:----------------------------------------------------|
|**Description**         |Unique identifier of data acquisition metadata block used to set this channel group. The acquisition_id must nest within specified interrogator_id. |
|**Required**            |True|
|**Type**                |String|
|**Style**               |Alphanumeric|
|**Units or options**    | -- |
|**Example**             |A001|

### cable_id
|attributeID              |<div align="right">cable_id <img width=200/> <code>Required</code> </div>|
|:------------------------|:----------------------------------------------------|
|**Description**         |Unique identifier of cable linked to this channel group. |
|**Required**            |True|
|**Type**                |String|
|**Style**               |Alphanumeric|
|**Units or options**    | -- |
|**Example**             |CA001|

### fiber_id
|attributeID              |<div align="right">fiber_id <img width=200/> <code>Required</code> </div>|
|:------------------------|:----------------------------------------------------|
|**Description**         |Unique identifier of fiber linked to this channel group. The fiber_id must nest within specified cable_id. |
|**Required**            |True|
|**Type**                |String|
|**Style**               |Alphanumeric|
|**Units or options**    | -- |
|**Example**             |F001|

### coordinate_generation_date
|attributeID              |<div align="right">coordinate_generation_date <img width=200/> <code>Required</code> </div>|
|:------------------------|:----------------------------------------------------|
|**Description**         |Date that the channel coordinates were generated.|
|**Required**            |True|
|**Type**                |String|
|**Style**               |ISO formatted datetime|
|**Units or options**    | -- |
|**Example**             |2016-07-01T00:00:00.000Z|

### coordinate_system
|attributeID              |<div align="right">coordinate_system <img width=200/> <code>Required</code> </div>|
|:------------------------|:----------------------------------------------------|
|**Description**         |Coordinate system used in channel location. Select geographic for coordinates in latitude and longitude. UTM is the preferred projected coordinate system. |
|**Required**            |True|
|**Type**                |String|
|**Style**               |Controlled vocabulary|
|**Units or options**    | [geographic | UTM | local ]|
|**Example**             | UTM |

### reference_frame
|attributeID              |<div align="right">reference_frame <img width=200/> <code>Required</code> </div>|
|:------------------------|:----------------------------------------------------|
|**Description**         |Geodetic datum and / or grid zone number in UTM.|
|**Required**            |True|
|**Type**                |String|
|**Style**               |Controlled vocabulary|
|**Units or options**    | [WGS84 | UTM Zone number]|
|**Example**             | UTM Zone 11N |

### distance_along_fiber_unit
|attributeID              |<div align="right">distance_along_fiber_unit <img width=200/> <code>Required</code> </div>|
|:------------------------|:----------------------------------------------------|
|**Description**         |Unit of distance along fiber.|
|**Required**            |True|
|**Type**                |String|
|**Style**               |Controlled vocabulary|
|**Units or options**    | meter |
|**Example**             | meter |

### x_coordinate_unit
|attributeID              |<div align="right">x_coordinate_unit <img width=200/> <code>Required</code> </div>|
|:------------------------|:----------------------------------------------------|
|**Description**         |Unit of x-coordinate (UTM-x or longitude). Applies to every individual channel nested under the channel group.|
|**Required**            |True|
|**Type**                |String|
|**Style**               |Controlled vocabulary|
|**Units or options**    | [decimal degree | meter] |
|**Example**             | meter |

### y_coordinate_unit
|attributeID              |<div align="right">y_coordinate_unit <img width=200/> <code>Required</code> </div>|
|:------------------------|:----------------------------------------------------|
|**Description**         |Unit of y-coordinate (UTM-y or latitude). Applies to every individual channel nested under the channel group.|
|**Required**            |True|
|**Type**                |String|
|**Style**               |Controlled vocabulary|
|**Units or options**    | [decimal degree | meter] |
|**Example**             | meter |

### location_method
|attributeID              |<div align="right">location_method <img width=200/> <code>Optional</code> </div>|
|:------------------------|:----------------------------------------------------|
|**Description**         |Method used to determine the coordinates of each channel. Example: tap test, GPS tracker.|
|**Required**            |False|
|**Type**                |String|
|**Style**               |Free form text|
|**Units or options**    | [tap test | GPS | other] |
|**Example**             | tap test |

### uncertainty_in_x_coordinate
|attributeID              |<div align="right">uncertainty_in_x_coordinate <img width=200/> <code>Optional</code> </div>|
|:------------------------|:----------------------------------------------------|
|**Description**         |Uncertainty in the x-coordinate (UTM-x or longitude), representing the average uncertainty for all the channels.|
|**Required**            |False|
|**Type**                |Float|
|**Style**               |na|
|**Units or options**    | - |
|**Example**             | - |

### uncertainty_in_x_coordinate_unit
|attributeID              |<div align="right">y_coordinate_unit <img width=200/> <code>Optional</code> </div>|
|:------------------------|:----------------------------------------------------|
|**Description**         |Unit of uncertainty in x-coordinate.|
|**Required**            |False|
|**Type**                |String|
|**Style**               |Controlled vocabulary|
|**Units or options**    | meter |
|**Example**             | meter |

### uncertainty_in_y_coordinate
|attributeID              |<div align="right">uncertainty_in_y_coordinate <img width=200/> <code>Optional</code> </div>|
|:------------------------|:----------------------------------------------------|
|**Description**         |Uncertainty in the y-coordinate, representing the average uncertainty for all the channels.|
|**Required**            |False|
|**Type**                |Float|
|**Style**               |na|
|**Units or options**    | - |
|**Example**             | - |

### uncertainty_in_y_coordinate_unit
|attributeID              |<div align="right">uncertainty_in_y_coordinate_unit <img width=200/> <code>Optional</code> </div>|
|:------------------------|:----------------------------------------------------|
|**Description**         |Unit of uncertainty in y-coordinate.|
|**Required**            |False|
|**Type**                |String|
|**Style**               |Controlled vocabulary|
|**Units or options**    | meter |
|**Example**             | meter |

### elevation_above_sea_level_unit
|attributeID              |<div align="right">elevation_above_sea_level_unit <img width=200/> <code>Optional</code> </div>|
|:------------------------|:----------------------------------------------------|
|**Description**         |Unit of elevation above sea level. Applies to every individual channel nested under the channel group.|
|**Required**            |False|
|**Type**                |String|
|**Style**               |Controlled vocabulary|
|**Units or options**    | meter |
|**Example**             | meter |

### uncertainty_in_elevation
|attributeID              |<div align="right">uncertainty_in_elevation <img width=200/> <code>Optional</code> </div>|
|:------------------------|:----------------------------------------------------|
|**Description**         |Uncertainty in elevation above sea level, representing the average uncertainty in elevation for all the coordinates.|
|**Required**            |False|
|**Type**                |Float|
|**Style**               |na|
|**Units or options**    | - |
|**Example**             | - |

### uncertainty_in_elevation_unit
|attributeID              |<div align="right">uncertainty_in_elevation_unit <img width=200/> <code>Optional</code> </div>|
|:------------------------|:----------------------------------------------------|
|**Description**         |Unit of uncertainty in elevation.|
|**Required**            |False|
|**Type**                |String|
|**Style**               |Controlled vocabulary|
|**Units or options**    | meter |
|**Example**             | meter |

### depth_below_surface_unit
|attributeID              |<div align="right">depth_below_surface_unit <img width=200/> <code>Optional</code> </div>|
|:------------------------|:----------------------------------------------------|
|**Description**         |Unit of depth below surface. Applies to every individual channel nested under the channel group.|
|**Required**            |False|
|**Type**                |String|
|**Style**               |Controlled vocabulary|
|**Units or options**    | meter |
|**Example**             | meter |

### uncertainty_in_depth
|attributeID              |<div align="right">uncertainty_in_depth <img width=200/> <code>Optional</code> </div>|
|:------------------------|:----------------------------------------------------|
|**Description**         |Uncertainty in depth below surface, representing the average uncertainty in depth for all the coordinates.|
|**Required**            |False|
|**Type**                |Float|
|**Style**               |na|
|**Units or options**    | - |
|**Example**             | - |

### uncertainty_in_depth_unit
|attributeID              |<div align="right">uncertainty_in_depth_unit <img width=200/> <code>Optional</code> </div>|
|:------------------------|:----------------------------------------------------|
|**Description**         |Unit of uncertainty in depth.|
|**Required**            |False|
|**Type**                |String|
|**Style**               |Controlled vocabulary|
|**Units or options**    | meter |
|**Example**             | meter |

### strike_unit
|attributeID              |<div align="right">strike_unit <img width=200/> <code>Optional</code> </div>|
|:------------------------|:----------------------------------------------------|
|**Description**         |Unit of strike. Defined at channel group level as it applies to every individual channel nested under the channel group.|
|**Required**            |False|
|**Type**                |String|
|**Style**               |Controlled vocabulary|
|**Units or options**    | degree |
|**Example**             | - |

### uncertainty_in_strike
|attributeID              |<div align="right">uncertainty_in_strike <img width=200/> <code>Optional</code> </div>|
|:------------------------|:----------------------------------------------------|
|**Description**         |Uncertainty in the strike in meters.|
|**Required**            |False|
|**Type**                |Float|
|**Style**               |na|
|**Units or options**    | - |
|**Example**             | - |

### uncertainty_in_strike_unit
|attributeID              |<div align="right">uncertainty_in_strike_unit <img width=200/> <code>Optional</code> </div>|
|:------------------------|:----------------------------------------------------|
|**Description**         |Unit of uncertainty in strike.|
|**Required**            |False|
|**Type**                |String|
|**Style**               |Controlled vocabulary|
|**Units or options**    | degree |
|**Example**             | - |

### dip_unit
|attributeID              |<div align="right">dip_unit <img width=200/> <code>Optional</code> </div>|
|:------------------------|:----------------------------------------------------|
|**Description**         |Unit of dip. Defined at channel group level as it applies to every individual channel nested under the channel group.|
|**Required**            |False|
|**Type**                |String|
|**Style**               |Controlled vocabulary|
|**Units or options**    | degree |
|**Example**             | - |

### uncertainty_in_dip
|attributeID              |<div align="right">uncertainty_in_dip <img width=200/> <code>Optional</code> </div>|
|:------------------------|:----------------------------------------------------|
|**Description**         |Uncertainty in the dip in meters.|
|**Required**            |False|
|**Type**                |Float|
|**Style**               |na|
|**Units or options**    | - |
|**Example**             | - |

### uncertainty_in_dip_unit
|attributeID              |<div align="right">uncertainty_in_dip_unit <img width=200/> <code>Optional</code> </div>|
|:------------------------|:----------------------------------------------------|
|**Description**         |Unit of uncertainty in dip.|
|**Required**            |False|
|**Type**                |String|
|**Style**               |Controlled vocabulary|
|**Units or options**    | degree |
|**Example**             | - |

### first_usable_channel_id
|attributeID              |<div align="right">first_usable_channel_id <img width=200/> <code>Optional</code> </div>|
|:------------------------|:----------------------------------------------------|
|**Description**         |The first channel considered physically meaningful. Typically, this will be a few channels after the last channel inside the interrogator. Must match one of the channel ids.|
|**Required**            |False|
|**Type**                |Integer|
|**Style**               |Alphanumeric|
|**Units or options**    | na |
|**Example**             | 30 |

### last_usable_channel_id
|attributeID              |<div align="right">last_usable_channel_id <img width=200/> <code>Optional</code> </div>|
|:------------------------|:----------------------------------------------------|
|**Description**         |The last channel considered physically meaningful. Typically, an acquisition will add virtual channels at the end of the fiber or the optical path might not reach the end of the fiber and this can be used to cut the dataset into a working set. Must match one of the channel ids.|
|**Required**            |False|
|**Type**                |Integer|
|**Style**               |Alphanumeric|
|**Units or options**    | na |
|**Example**             | 8650 |

### comment
|attributeID              |<div align="right">comment <img width=200/> <code>Optional</code> </div>|
|:------------------------|:----------------------------------------------------|
|**Description**         |Additional comments.|
|**Required**            |False|
|**Type**                |String|
|**Style**               |Free form text|
|**Units or options**    | --
|**Example**             |na|
