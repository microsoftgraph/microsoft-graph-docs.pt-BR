---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 79adb9e95d1c886649e1782b796347205a8f030d
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/10/2020
ms.locfileid: "44685186"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var printUserIdentity = new PrintUserIdentity
{
    AdditionalData = new Dictionary<string, object>()
    {
        {"@odata.id", "https://graph.microsoft.com/beta/users/{id}"}
    }
};

await graphClient.Print.Shares["{id}"].AllowedUsers.References
    .Request()
    .AddAsync(printUserIdentity);

```