---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f0ef073f9b37062c6c19e7e77237538c8dd36025
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62115076"
---
```powershell

Import-Module Microsoft.Graph.Education

$params = @{
    "@odata.type" = "#microsoft.graph.educationClass"
    DisplayName = "String"
    MailNickname = "String"
    Description = "String"
    CreatedBy = @{
        "@odata.type" = "microsoft.graph.identitySet"
    }
    ClassCode = "String"
    ExternalName = "String"
    ExternalId = "String"
    ExternalSource = "String"
    ExternalSourceDetail = "String"
    Grade = "String"
    Term = @{
        "@odata.type" = "microsoft.graph.educationTerm"
    }
}

New-MgEducationClass -BodyParameter $params

```