---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 64fe762f8d6973d6f873dda82132beef003e428f7016719e059398c4f18ede83
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57217337"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var chatMessageHostedContent = await graphClient.Chats["{chat-id}"].Messages["{chatMessage-id}"].HostedContents["{chatMessageHostedContent-id}"]
    .Request()
    .GetAsync();

```