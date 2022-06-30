---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 18981fb8abd0b9ae763d237916217086ab82997d
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/29/2022
ms.locfileid: "66443934"
---
```powershell

Import-Module Microsoft.Graph.DeviceManagement.Enrolment

Get-MgRoleManagementDirectoryRoleAssignmentScheduleRequest -Property "principalId,action,roleDefinitionId" -ExpandProperty "roleDefinition,activatedUsing,principal,targetSchedule" 

```