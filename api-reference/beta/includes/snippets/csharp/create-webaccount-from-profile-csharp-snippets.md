---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2a501371ce892e617d8cd2305093c55f96d0de38
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/05/2019
ms.locfileid: "37996463"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var webAccount = new WebAccount
{
    Description = "description-value",
    UserId = "userId-value",
    Service = new ServiceInformation
    {
        Name = "name-value",
        WebUrl = "webUrl-value"
    },
    StatusMessage = "statusMessage-value",
    WebUrl = "webUrl-value"
};

await graphClient.Me.Profile.WebAccounts
    .Request()
    .AddAsync(webAccount);

```