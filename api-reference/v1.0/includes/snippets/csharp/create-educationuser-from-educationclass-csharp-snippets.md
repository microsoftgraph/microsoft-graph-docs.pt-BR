---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bab73888965bdc1e51be46756eab19de31cb48ad
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35881537"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationUser = new EducationUser
{
    AdditionalData = new Dictionary<string, object>()
    {
        {"@odata.id","https://graph.microsoft.com/v1.0/education/users/14011"}
    }
};

await graphClient.Education.Classes["{class-id}"].Teachers.References
    .Request()
    .AddAsync(educationUser);

```