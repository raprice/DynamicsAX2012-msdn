﻿---
title: ReleaseUpdateDB60_Invent.allowDupInvtFsclLIFOJrnllTrnsAdjGrpIdx Upgrade Script
TOCTitle: ReleaseUpdateDB60_Invent.allowDupInvtFsclLIFOJrnllTrnsAdjGrpIdx Upgrade Script
ms:assetid: 2a1403cc-3fe9-8bef-d08a-84f3f8d19e75
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/JJ735905(v=AX.60)
ms:contentKeyID: 49707322
ms.date: 05/18/2015
mtps_version: v=AX.60
---

# ReleaseUpdateDB60\_Invent.allowDupInvtFsclLIFOJrnllTrnsAdjGrpIdx Upgrade Script 


_**Applies To:** Microsoft Dynamics AX 2012 R3, Microsoft Dynamics AX 2012 R2, Microsoft Dynamics AX 2012 Feature Pack, Microsoft Dynamics AX 2012_

<table>
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><strong>Class</strong></p></td>
<td><p>ReleaseUpdateDB60_Invent</p></td>
</tr>
<tr class="even">
<td><p><strong>Method</strong></p></td>
<td><p>allowDupInvtFsclLIFOJrnllTrnsAdjGrpIdx</p></td>
</tr>
<tr class="odd">
<td><p><strong>Description</strong></p></td>
<td><p>Updates the GroupItemYearIdx index in the InventFiscalLIFOJournalTransAdj table to allow for duplicate records.</p></td>
</tr>
</tbody>
</table>


## Affected Modules and Tables

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<thead>
<tr class="header">
<th><p>Affected Modules</p></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p>General ledger</p></td>
</tr>
</tbody>
</table>


<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<thead>
<tr class="header">
<th><p>Affected Tables</p></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p>InventFiscalLIFOJournalTransAdj</p></td>
</tr>
</tbody>
</table>


## Remarks

The name of this method is truncated from allowDupInventFiscalLIFOJournalTransAdjGroupItemYearIdx. The FiscalLIFOGroupId field is replaced with the new surrogate key InventFiscalLIFOGroup field in the unique GroupItemYearIdx index. Initially, this field contains no value. Therefore, the index is set to allow for duplicates before the field is updated with the value of the RecId field of the InventFiscalLIFOGroup table.

  
**Announcements:** To see known issues and recent fixes, use [Issue search](http://go.microsoft.com/fwlink/?linkid=389258) in [Microsoft Dynamics Lifecycle Services](http://go.microsoft.com/fwlink/?linkid=306505) (LCS).
