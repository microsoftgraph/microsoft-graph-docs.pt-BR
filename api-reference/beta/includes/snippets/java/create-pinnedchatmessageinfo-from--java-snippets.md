---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 095ffcc754af3a09730aca35e7c2d2e48a167332
ms.sourcegitcommit: 54ba08a80db85b9e84813387e8c4416eca44fa8e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/26/2022
ms.locfileid: "65693857"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PinnedChatMessageInfo pinnedChatMessageInfo = new PinnedChatMessageInfo();
pinnedChatMessageInfo.additionalDataManager().put("message@odata.bind", new JsonPrimitive("https://graph.microsoft.com/beta/chats/19:2da4c29f6d7041eca70b638b43d45437@thread.v2/messages/1616964509832"));

graphClient.chats("19:2da4c29f6d7041eca70b638b43d45437@thread.v2").pinnedMessages()
    .buildRequest()
    .post(pinnedChatMessageInfo);

```