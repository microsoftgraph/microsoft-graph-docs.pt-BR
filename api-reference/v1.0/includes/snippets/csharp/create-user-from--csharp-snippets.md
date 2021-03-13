---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f152f3005116526bc947eb17c814c1a76420ee97
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50771432"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var user = new User
{
    AdditionalData = new Dictionary<string, object>()
    {
        {"@odata.id", "https://graph.microsoft.com/v1.0/users/{userId}"}
    }
};

await graphClient.Print.Shares["{printerShare-id}"].AllowedUsers.References
    .Request()
    .AddAsync(user);

```