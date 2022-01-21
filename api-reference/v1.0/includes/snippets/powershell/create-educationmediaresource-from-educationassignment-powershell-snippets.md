---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fae41722a2947143155d24ad27275429a35dc668
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62128812"
---
```powershell

Import-Module Microsoft.Graph.Education

$params = @{
    DistributeForStudentWork = $false
    Resource = @{
        "@odata.type" = "microsoft.graph.educationMediaResource"
        DisplayName = "homework example.PNG"
        FileUrl = "https://graph.microsoft.com/v1.0/drives/b!OPmUsPgnBUiMIXMxWcj3neC1xck6I5NIsnFxfrLdmXoOOmEQNO79QpIMPdOmY3nf/items/01QTY63RMUWOKAGSJZ6BHINJVKNMOOJABF"
    }
}

New-MgEducationClassAssignmentResource -EducationClassId $educationClassId -EducationAssignmentId $educationAssignmentId -BodyParameter $params

```