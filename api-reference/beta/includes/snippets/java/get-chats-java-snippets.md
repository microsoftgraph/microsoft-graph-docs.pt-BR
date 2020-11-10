---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 29ab3c17d304c5135e36ba7bdef1a19d0568218f
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48951528"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IChatCollectionPage chats = graphClient.users("{id}").chats()
    .buildRequest()
    .get();

```