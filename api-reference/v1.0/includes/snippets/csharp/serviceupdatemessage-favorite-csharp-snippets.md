---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f3ccffec5d454f9fcf4689e53b2738e102ec4036
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58266654"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var messageIds = new List<String>()
{
    "MC172851",
    "MC167983"
};

await graphClient.Admin.ServiceAnnouncement.Messages
    .Favorite(messageIds)
    .Request()
    .PostAsync();

```