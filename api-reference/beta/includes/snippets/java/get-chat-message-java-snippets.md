---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b1fe4664006f7a6b7b5ab3a7e0048095a1b040d8
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50975485"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ChatMessage chatMessage = graphClient.me().chats("{id}").messages("{id}")
    .buildRequest()
    .get();

```