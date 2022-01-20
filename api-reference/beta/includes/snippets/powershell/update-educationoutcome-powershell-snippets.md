---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: eac003ca383c8ffdf3b808882d51e84b30741cc0
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62137190"
---
```powershell

Import-Module Microsoft.Graph.Education

$params = @{
    "@odata.type" = "#microsoft.graph.educationRubricOutcome"
    RubricQualityFeedback = @(
    )
    RubricQualitySelectedLevels = @(
    )
}

Update-MgEducationClassAssignmentSubmissionOutcome -EducationClassId $educationClassId -EducationAssignmentId $educationAssignmentId -EducationSubmissionId $educationSubmissionId -EducationOutcomeId $educationOutcomeId -BodyParameter $params

```