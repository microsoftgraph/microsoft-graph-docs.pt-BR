---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ce70d3a76075aa4841cc8fa407570b3584957455
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62131365"
---
```powershell

Import-Module Microsoft.Graph.Compliance

$params = @{
    Email = "AdeleV@contoso.com"
    ApplyHoldToSources = "true"
}

New-MgComplianceEdiscoveryCaseCustodian -CaseId $caseId -BodyParameter $params

```