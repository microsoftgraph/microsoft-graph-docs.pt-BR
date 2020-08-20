---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 86d5c299c40502704d8d4199cd462a13ab72117a
ms.sourcegitcommit: 239db9e961e42b505f52de9859963a9136935f2f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/20/2020
ms.locfileid: "46821162"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var webAccount = new WebAccount
{
    Description = "My Github contributions!",
    UserId = "innocenty.popov",
    Service = new ServiceInformation
    {
        Name = "GitHub",
        WebUrl = "https://github.com"
    }
};

await graphClient.Me.Profile.WebAccounts
    .Request()
    .AddAsync(webAccount);

```