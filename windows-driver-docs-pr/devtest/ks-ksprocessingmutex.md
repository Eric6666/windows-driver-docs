---
title: KsProcessingMutex rule ()
ms.assetid: AD73B241-7B08-4E48-94A1-B6BDE78590E6
ms.author: windowsdriverdev
ms.date: 5/21/2018
ms.topic: article
ms.prod: windows-hardware
ms.technology: windows-devices
description: 
keywords: ["KsProcessingMutex rule ()"]
topic_type:
- apiref
api_name:
- KsProcessingMutex
api_type:
- NA
---

# KsProcessingMutex rule ()


The KsProcessingMutex rule specifies that a KS miniport driver uses the processing mutex in the correct sequence:

-   The processing mutex cannot be obtained recursively.
-   A thread that has acquired the processing mutex should not subsequently attempt to acquire the filter control mutex.
-   A thread should not release the processing mutex without acquiring it first.

|              |     |
|--------------|-----|
| Driver model | KS  |

|                                   |                                                                                                                                       |
|-----------------------------------|---------------------------------------------------------------------------------------------------------------------------------------|
| Bug check(s) found with this rule | [**Bug Check 0xC4: DRIVER\_VERIFIER\_DETECTED\_VIOLATION**](https://msdn.microsoft.com/library/windows/hardware/ff560187) (0x0008100B) |

How to test
-----------

<table>
<colgroup>
<col width="100%" />
</colgroup>
<thead>
<tr class="header">
<th align="left">At run time</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td align="left"><p>To verify this rule, open a Command Prompt window. Enter a Driver Verifier command and specify <strong>/domain ks</strong>.</p>
<p>For example:</p>
<p><strong>verifier /domain ks</strong> [<em>options</em>] <strong>/driver</strong> <em>&lt;yourdriver&gt;</em></p>
<p>For more information, see [Driver Verifier](https://msdn.microsoft.com/library/windows/hardware/ff545448).</p></td>
</tr>
</tbody>
</table>

 

See also
--------

[Processing Mutex in AVStream](https://msdn.microsoft.com/library/windows/hardware/ff567790)
 

 





