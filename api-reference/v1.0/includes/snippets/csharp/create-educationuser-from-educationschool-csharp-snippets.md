---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fdb2bd6f4cbd5a1404453bfc19ef21e34e5fa357
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/10/2020
ms.locfileid: "44684776"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationUser = new EducationUser
{
    AdditionalData = new Dictionary<string, object>()
    {
        {"@odata.id", "https://graph.microsoft.com/v1.0/education/users/14008"}
    }
};

await graphClient.Education.Schools["{id}"].Users.References
    .Request()
    .AddAsync(educationUser);

```