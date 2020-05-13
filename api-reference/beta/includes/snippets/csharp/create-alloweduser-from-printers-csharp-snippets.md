---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 82a3a3583d7e2f4ce6d2326188e6691d70f890d1
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2020
ms.locfileid: "44216753"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var printUserIdentity = new PrintUserIdentity
{
    AdditionalData = new Dictionary<string, object>()
    {
        {"@odata.id","https://graph.microsoft.com/beta/users/{id}"}
    }
};

await graphClient.Print.Shares["{id}"].AllowedUsers.References
    .Request()
    .AddAsync(printUserIdentity);

```