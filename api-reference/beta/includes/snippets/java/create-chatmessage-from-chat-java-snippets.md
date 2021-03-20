---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 560eca121408c12238607f59f1ed17f10256727c
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50977943"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ChatMessage chatMessage = new ChatMessage();
ItemBody body = new ItemBody();
body.content = "Hello world";
chatMessage.body = body;

graphClient.chats("{id}").messages()
    .buildRequest()
    .post(chatMessage);

```