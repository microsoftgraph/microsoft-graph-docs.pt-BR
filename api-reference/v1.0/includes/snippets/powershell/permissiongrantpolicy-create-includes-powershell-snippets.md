---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6177cb806933e0775694e6e850f5e9970e5325e1
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62124575"
---
```powershell

Import-Module Microsoft.Graph.Identity.SignIns

$params = @{
    PermissionType = "delegated"
    ClientApplicationsFromVerifiedPublisherOnly = $true
}

New-MgPolicyPermissionGrantPolicyInclude -PermissionGrantPolicyId $permissionGrantPolicyId -BodyParameter $params

```