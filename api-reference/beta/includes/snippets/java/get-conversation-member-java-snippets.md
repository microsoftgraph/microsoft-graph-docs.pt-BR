---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b12889520818a88defc2d675e54050f8e6bec117
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48956740"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ConversationMember conversationMember = graphClient.chats("{id}").members("{id}")
    .buildRequest()
    .get();

```