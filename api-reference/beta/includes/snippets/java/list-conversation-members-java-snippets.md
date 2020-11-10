---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f5b8acd99cc7ae5430e21e5e579ecc5beb91f2dc
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48956726"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IConversationMemberCollectionPage members = graphClient.me().chats("{id}").members()
    .buildRequest()
    .get();

```