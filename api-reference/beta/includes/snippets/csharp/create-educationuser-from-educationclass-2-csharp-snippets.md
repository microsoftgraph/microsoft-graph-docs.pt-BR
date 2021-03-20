---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fb9f89b07b824db0cf48c768b770f50e255594c4
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50951514"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationUser = new EducationUser
{
    AdditionalData = new Dictionary<string, object>()
    {
        {"@odata.id", "https://graph.microsoft.com/beta/education/users/14011"}
    }
};

await graphClient.Education.Classes["{educationClass-id}"].Teachers.References
    .Request()
    .AddAsync(educationUser);

```