---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e238146dca4fbda4bf13fd1a7233a5b2d343f842
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/29/2022
ms.locfileid: "66441620"
---
```powershell

Import-Module Microsoft.Graph.DeviceManagement.Enrolment

Get-MgRoleManagementDirectoryRoleAssignmentScheduleRequest -UnifiedRoleAssignmentScheduleRequestId $unifiedRoleAssignmentScheduleRequestId -Property "principalId,action,roleDefinitionId" -ExpandProperty "roleDefinition,activatedUsing,principal,targetSchedule" 

```