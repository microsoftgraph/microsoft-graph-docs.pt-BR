---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e4ff0408deb25f6dca9cfdfaf0200648691a79fc
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62088877"
---
```powershell

Import-Module Microsoft.Graph.Identity.DirectoryManagement

$params = @{
    RoleId = "roleId-value"
    RoleMemberInfo = @{
        Id = "id-value"
    }
}

New-MgDirectoryAdministrativeUnitScopedRoleMember -AdministrativeUnitId $administrativeUnitId -BodyParameter $params

```