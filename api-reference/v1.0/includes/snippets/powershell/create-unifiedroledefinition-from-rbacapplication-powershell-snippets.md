---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 249bb06877ae5e1040a83e434c3b67f96c1abd71
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62134389"
---
```powershell

Import-Module Microsoft.Graph.DeviceManagement.Enrolment

$params = @{
    Description = "Update basic properties of application registrations"
    DisplayName = "Application Registration Support Administrator"
    RolePermissions = @(
        @{
            AllowedResourceActions = @(
                "microsoft.directory/applications/basic/read"
            )
        }
    )
    IsEnabled = $true
}

New-MgRoleManagementDirectoryRoleDefinition -BodyParameter $params

```