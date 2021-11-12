---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2183019ef8cbb4b0e20ed77bb4692f8d1bf1b7c4ebc19c99fa5b4c531f59829b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57214780"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var user = new User
{
    AdditionalData = new Dictionary<string, object>()
    {
        {"@odata.id", "https://graph.microsoft.com/beta/users/{id}"}
    }
};

await graphClient.Print.Shares["{printerShare-id}"].AllowedUsers.References
    .Request()
    .AddAsync(user);

```