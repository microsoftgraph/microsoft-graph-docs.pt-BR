---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ed4159acb697e788923691baeca6a9a267a26553
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62136475"
---
```powershell

Import-Module Microsoft.Graph.Applications

$params = @{
    "@odata.id" = "https://graph.microsoft.com/v1.0/policies/tokenIssuancePolicies/cd3d9b57-0aee-4f25-8ee3-ac74ef5986a9"
}

New-MgApplicationTokenIssuancePolicyByRef -ApplicationId $applicationId -BodyParameter $params

```