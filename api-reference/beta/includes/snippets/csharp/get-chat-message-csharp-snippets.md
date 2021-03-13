---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 10d0a8055618bf327e237430fc9917ddd45eacca
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50790409"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var chatMessage = await graphClient.Me.Chats["{chat-id}"].Messages["{chatMessage-id}"]
    .Request()
    .GetAsync();

```