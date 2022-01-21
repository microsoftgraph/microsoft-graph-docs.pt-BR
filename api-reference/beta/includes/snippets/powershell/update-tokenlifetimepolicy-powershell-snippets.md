---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 00ad654c53ed76d086d2eb79ad66b56ecfa95447
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62136887"
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

Update-MgPolicyTokenLifetimePolicy -TokenLifetimePolicyId $tokenLifetimePolicyId -BodyParameter $params

```