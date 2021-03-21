---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4428429f1ef0f93339389a382675b179db35621b
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50958269"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var chat = new Chat
{
    Topic = "Group chat title update"
};

await graphClient.Chats["{chat-id}"]
    .Request()
    .UpdateAsync(chat);

```