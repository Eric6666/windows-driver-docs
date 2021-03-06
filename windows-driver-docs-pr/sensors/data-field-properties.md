---
title: Data field properties
description: This topic describes the sensor properties that are used for data fields only.
ms.assetid: A7FA02AA-7B7B-45B4-A432-4B4ED69CB19C
ms.author: windowsdriverdev
ms.date: 01/04/2018
ms.topic: article
ms.prod: windows-hardware
ms.technology: windows-devices
---

# Data field properties


This topic describes the sensor properties that are used for data fields only.

The following table shows the sensor properties. Because these properties apply to any data-field, the type can vary depending on which data-field these properties are referring to, see the [Sensor data fields](sensor-data-fields.md) topic for more information.

<table>
<colgroup>
<col width="20%" />
<col width="20%" />
<col width="20%" />
<col width="20%" />
<col width="20%" />
</colgroup>
<thead>
<tr class="header">
<th>Property key</th>
<th>Type</th>
<th>Access (R/O, R/W)</th>
<th>Required/Optional</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p>PKEY_SensorDataField_Resolution</p></td>
<td><p>See the data field type.</p></td>
<td><p>R/O</p></td>
<td><p>This depends on the data fields, for a list of property keys that require this data field see the [Required data field properties](required-data-field-properties.md) topic.</p></td>
<td><p>The resolution of the data field.</p></td>
</tr>
<tr class="even">
<td><p>PKEY_SensorDataField_RangeMinimum</p></td>
<td><p>See the data field type.</p></td>
<td><p>R/O</p></td>
<td><p>This depends on the data fields, for a list of property keys that require this data field see the [Required data field properties](required-data-field-properties.md) topic.</p></td>
<td><p>The minimum value of the data field.</p></td>
</tr>
<tr class="odd">
<td><p>PKEY_SensorDataField_RangeMaximum</p></td>
<td><p>See the data field type.</p></td>
<td><p>R/O</p></td>
<td><p>This depends on the data fields, for a list of property keys that require this data field see the [Required data field properties](required-data-field-properties.md) topic.</p></td>
<td><p>The maximum value of the data field.</p></td>
</tr>
</tbody>
</table>

 

## <span id="Requirements"></span><span id="requirements"></span><span id="REQUIREMENTS"></span>Requirements


**Header:** Sensorsdef.h

## <span id="related_topics"></span>Related topics


[Required data field properties](required-data-field-properties.md)

[Sensor data fields](sensor-data-fields.md)

[Sensor properties](sensor-properties2.md)

 

 






