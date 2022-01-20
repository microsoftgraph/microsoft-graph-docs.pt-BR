---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4894aa35d8950b077b8788cc1f68616d613464d1
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62111491"
---
```powershell

Import-Module Microsoft.Graph.Applications

$params = @{
    "@odata.id" = "https://graph.microsoft.com/v1.0/policies/tokenLifetimePolicies/cd3d9b57-0aee-4f25-8ee3-ac74ef5986a9"
}

New-MgApplicationTokenLifetimePolicyByRef -ApplicationId $applicationId -BodyParameter $params

```