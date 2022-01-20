---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: dd1ff9b1b68611049fee00ff4298c063754ba402
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62123252"
---
```powershell

Import-Module Microsoft.Graph.Identity.SignIns

$params = @{
    PermissionType = "delegated"
    ResourceApplication = "00000003-0000-0000-c000-000000000000"
}

New-MgPolicyPermissionGrantPolicyExclude -PermissionGrantPolicyId $permissionGrantPolicyId -BodyParameter $params

```