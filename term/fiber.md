**Fiber Metadata**
*  The intention for a separate Fiber metadata is to uniquely identify the fiber used to make the measurements. More than one cable may be used over the course of an experiment and there may be several fibers within a cable.

* Required fields *(mark with an asterisk, and indicated in the tables below)* \
[fiber_id*](#fiber_id) |
[cable_id*](#cable_id) |
[fiber_geometry*](#fiber_geometry) |
[fiber_mode*](#fiber_mode) |
[fiber_refraction_index*](#fiber_refraction_index)

* Optional fields\
[fiber_winding_angle](#fiber_winding_angle) |
[fiber_winding_angle_unit](#fiber_winding_angle_unit) |
[fiber_start_location](#fiber_start_location) |
[fiber_start_location_unit](#fiber_start_location_unit) |
[fiber_end_location](#fiber_end_location) |
[fiber_end_location_unit](#fiber_end_location_unit) |
[fiber_optical_length](#fiber_optical_length) |
[fiber_optical_length_unit](#fiber_optical_length_unit) |
[fiber_one_way_attenuation](#fiber_one_way_attenuation) |
[fiber_one_way_attenuation_unit](#fiber_one_way_attenuation_unit) |
[comment](#comment)

---
### fiber_id
|attributeID              |<div align="right">fiber_id <img width=200/> <code>Required</code> </div>|
|:------------------------|:----------------------------------------------------|
|**Description**         |Unique identifier for the physical fiber, with a maximum of 8 alphanumeric characters with no special characters (e.g., underscores, period, dash). |
|**Required**            |True|
|**Type**                |String|
|**Style**               |Alphanumeric|
|**Units or options**    | -- |
|**Example**             |F001|

### cable_id
|attributeID              |<div align="right">cable_id <img width=200/> <code>Required</code> </div>|
|:------------------------|:----------------------------------------------------|
|**Description**         |Unique identifier associates this fiber to a specific cable. |
|**Required**            |True|
|**Type**                |String|
|**Style**               |Alphanumeric|
|**Units or options**    | -- |
|**Example**             |CA001|

### fiber_geometry
|attributeID              |<div align="right">fiber_geometry <img width=200/> <code>Required</code> </div>|
|:------------------------|:----------------------------------------------------|
|**Description**         |Geometry of fiber.|
|**Required**            | True|
|**Type**                |String|
|**Style**               |Controlled vocabulary|
|**Units or options**    | [linear | helical | other] |
|**Example**             | linear |

### fiber_mode
|attributeID              |<div align="right">fiber_mode <img width=200/> <code>Required</code> </div>|
|:------------------------|:----------------------------------------------------|
|**Description**         |Mode of fiber.|
|**Required**            | True|
|**Type**                |String|
|**Style**               |Controlled vocabulary|
|**Units or options**    | [single-mode | multi-mode | other ] |
|**Example**             | linear |

### fiber_refraction_index
|attributeID              |<div align="right">fiber_refraction_index <img width=200/> <code>Required</code> </div>|
|:------------------------|:----------------------------------------------------|
|**Description**         |Refractive index of the fiber (unitless). Typical value for single mode fiber is 1.4681.|
|**Required**            |True|
|**Type**                |Float|
|**Style**               |na|
|**Units or options**    | - |
|**Example**             | 1.4681 |

### fiber_winding_angle
|attributeID              |<div align="right">fiber_winding_angle <img width=200/> <code>Optional</code> </div>|
|:------------------------|:----------------------------------------------------|
|**Description**         |If helical, this is the winding angle relative to the center of the cable.|
|**Required**            |False|
|**Type**                |Float|
|**Style**               |na|
|**Units or options**    | - |
|**Example**             | - |

### fiber_winding_angle_unit
|attributeID              |<div align="right">fiber_winding_angle_unit <img width=200/> <code>Optional</code> </div>|
|:------------------------|:----------------------------------------------------|
|**Description**         |Unit of fibre winding angle|
|**Required**            |False|
|**Type**                |String|
|**Style**               |Controlled vocabulary|
|**Units or options**    | degree |
|**Example**             | - |

### fiber_start_location
|attributeID              |<div align="right">fiber_start_location <img width=200/> <code>Optional</code> </div>|
|:------------------------|:----------------------------------------------------|
|**Description**         |The start distance along the fiber with respect to the interrogator, referred to as StartLocus in PRODML.|
|**Required**            |False|
|**Type**                |Float|
|**Style**               |na|
|**Units or options**    | - |
|**Example**             | - |

### fiber_start_location_unit
|attributeID              |<div align="right">fiber_start_location_unit <img width=200/> <code>Optional</code> </div>|
|:------------------------|:----------------------------------------------------|
|**Description**         |Unit of fiber start location.|
|**Required**            | False|
|**Type**                |String|
|**Style**               |Controlled vocabulary|
|**Units or options**    | [meter | kilometer] |
|**Example**             | meter |

### fiber_start_location
|attributeID              |<div align="right">fiber_start_location <img width=200/> <code>Optional</code> </div>|
|:------------------------|:----------------------------------------------------|
|**Description**         |The start distance along the fiber with respect to the interrogator, referred to as StartLocus in PRODML.|
|**Required**            |False|
|**Type**                |Float|
|**Style**               |na|
|**Units or options**    | - |
|**Example**             | - |

### fiber_start_location_unit
|attributeID              |<div align="right">fiber_start_location_unit <img width=200/> <code>Optional</code> </div>|
|:------------------------|:----------------------------------------------------|
|**Description**         |Unit of fiber start location.|
|**Required**            |False|
|**Type**                |String|
|**Style**               |Controlled vocabulary|
|**Units or options**    | [meter | kilometer] |
|**Example**             | meter |

### fiber_end_location
|attributeID              |<div align="right">fiber_end_location <img width=200/> <code>Optional</code> </div>|
|:------------------------|:----------------------------------------------------|
|**Description**         |The end location or distance along the fiber with respect to the interrogator.|
|**Required**            |False|
|**Type**                |Float|
|**Style**               |na|
|**Units or options**    | - |
|**Example**             | - |

### fiber_end_location_unit
|attributeID              |<div align="right">fiber_end_location_unit <img width=200/> <code>Optional</code> </div>|
|:------------------------|:----------------------------------------------------|
|**Description**         |Unit of fiber end location.|
|**Required**            |False|
|**Type**                |String|
|**Style**               |Controlled vocabulary|
|**Units or options**    | [meter | kilometer] |
|**Example**             | meter |

### fiber_optical_length
|attributeID              |<div align="right">fiber_optical_length <img width=200/> <code>Optional</code> </div>|
|:------------------------|:----------------------------------------------------|
|**Description**         |Total length of this fiber. Typically, it is the sum of fiber_start_location and fiber_end_location.|
|**Required**            |False|
|**Type**                |Float|
|**Style**               |na|
|**Units or options**    | - |
|**Example**             | 8400 |

### fiber_optical_length_unit
|attributeID              |<div align="right">fiber_optical_length_unit <img width=200/> <code>Optional</code> </div>|
|:------------------------|:----------------------------------------------------|
|**Description**         |Unit of fiber optical length.|
|**Required**            |False|
|**Type**                |String|
|**Style**               |Controlled vocabulary|
|**Units or options**    | [meter | kilometer] |
|**Example**             | meter |

### fiber_one_way_attenuation
|attributeID              |<div align="right">fiber_one_way_attenuation <img width=200/> <code>Optional</code> </div>|
|:------------------------|:----------------------------------------------------|
|**Description**         |Power loss for one-way travel of a beam of light. Typical value for single mode fiber is 0.4.|
|**Required**            |False|
|**Type**                |Float|
|**Style**               |na|
|**Units or options**    | - |
|**Example**             | - |

### fiber_one_way_attenuation_unit
|attributeID              |<div align="right">fiber_one_way_attenuation_unit <img width=200/> <code>Optional</code> </div>|
|:------------------------|:----------------------------------------------------|
|**Description**         |Unit of fiber optical length.|
|**Required**            |False|
|**Type**                |String|
|**Style**               |Controlled vocabulary|
|**Units or options**    | [decibels/meter | decibels/kilometer] |
|**Example**             | - |

### comment
|attributeID              |<div align="right">comment <img width=200/> <code>Optional</code> </div>|
|:------------------------|:----------------------------------------------------|
|**Description**         |Additional comments.|
|**Required**            |False|
|**Type**                |String|
|**Style**               |Free form text|
|**Units or options**    | -- |
|**Example**             |na|
