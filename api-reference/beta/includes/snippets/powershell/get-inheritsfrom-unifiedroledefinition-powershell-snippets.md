---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e14f156d32b4d06d436f95dc0dd2076791478c6e
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62098442"
---
```powershell

Import-Module Microsoft.Graph.DeviceManagement.Enrolment

Get-MgRoleManagementDirectoryRoleDefinition -UnifiedRoleDefinitionId $unifiedRoleDefinitionId -ExpandProperty "inheritsPermissionsFrom" 

```