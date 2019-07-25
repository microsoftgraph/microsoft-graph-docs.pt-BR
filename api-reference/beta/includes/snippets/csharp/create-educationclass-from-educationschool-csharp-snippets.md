---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6b838bdd88daf47255ceea050e7ef6a7cdd02aa9
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35860222"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationClass = new EducationClass
{
    AdditionalData = new Dictionary<string, object>()
    {
        {"@odata.id","https://graph.microsoft.com/beta/education/classes/11006"}
    }
};

await graphClient.Education.Schools["10002"].Classes.References
    .Request()
    .AddAsync(educationClass);

```