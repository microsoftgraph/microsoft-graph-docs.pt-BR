---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 805c61c8abbadabbb492f715a3f2b133dacd84ab
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62110917"
---
```powershell

Import-Module Microsoft.Graph.Identity.SignIns

$params = @{
    Definition = @(
        "definition-value"
    )
    DisplayName = "displayName-value"
    IsOrganizationDefault = $true
}

New-MgPolicyHomeRealmDiscoveryPolicy -BodyParameter $params

```