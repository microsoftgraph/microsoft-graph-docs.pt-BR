---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0a4feb3cd166745e68eec1e1b3832c8b6c6430fa
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2021
ms.locfileid: "52254276"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationOutcome = new EducationPointsOutcome
{
    Points = new EducationAssignmentPointsGrade
    {
        Points = 85f
    }
};

await graphClient.Education.Classes["{educationClass-id}"].Assignments["{educationAssignment-id}"].Submissions["{educationSubmission-id}"].Outcomes["{educationOutcome-id}"]
    .Request()
    .UpdateAsync(educationOutcome);

```