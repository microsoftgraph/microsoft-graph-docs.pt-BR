---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a5727fa34d0e3d1912854174ed1e3a5a006e2a52
ms.sourcegitcommit: a1675c7b8dfc7d7c3c7923d06cda2b0127f9c3e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/05/2021
ms.locfileid: "49756132"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ChatMessage chatMessage = new ChatMessage();
ItemBody body = new ItemBody();
body.content = "Hello world";
chatMessage.body = body;

graphClient.chats("{id}").messages()
    .buildRequest()
    .post(chatMessage);

```