---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 324fe7536c3f5eb2434ebf8c8dfc1c96b0ce1b5c984688d4d8aa7c361e78d272
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56899278"
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