---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 54eb07bcc8d624d08a4d95b3c37b7c7489fb6663
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62137189"
---
```powershell

Import-Module Microsoft.Graph.Education

$params = @{
    "@odata.type" = "#microsoft.graph.educationFeedbackOutcome"
}

Update-MgEducationClassAssignmentSubmissionOutcome -EducationClassId $educationClassId -EducationAssignmentId $educationAssignmentId -EducationSubmissionId $educationSubmissionId -EducationOutcomeId $educationOutcomeId -BodyParameter $params

```