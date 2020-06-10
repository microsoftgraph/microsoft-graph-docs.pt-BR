---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 287468a56e75c732a995498886da367318a65808
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/10/2020
ms.locfileid: "44684423"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationRubric = new EducationRubric
{
    AdditionalData = new Dictionary<string, object>()
    {
        {"@odata.id", "https://graph.microsoft.com/v1.0/education/me/rubrics/{id}"}
    }
};

await graphClient.Education.Classes["{id}"].Assignments["{id}"].Rubric.Reference
    .Request()
    .PutAsync(educationRubric);

```