---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 27782addf96bd1ee1298044f90a310ac85d07842
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62131351"
---
```powershell

Import-Module Microsoft.Graph.Compliance

$params = @{
    "@odata.type" = "#microsoft.graph.ediscovery.legalHold"
    Description = "String"
    CreatedBy = @{
        "@odata.type" = "microsoft.graph.identitySet"
    }
    IsEnabled = "Boolean"
    Status = "String"
    ContentQuery = "String"
    Errors = @(
        "String"
    )
    DisplayName = "String"
}

New-MgComplianceEdiscoveryCaseLegalHold -CaseId $caseId -BodyParameter $params

```