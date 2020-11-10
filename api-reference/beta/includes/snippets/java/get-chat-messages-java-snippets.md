---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: de70c40c8727f42226e0a3e3e2fbefd3c1bb2aa5
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48958294"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IChatMessageCollectionPage messages = graphClient.chats("{id}").messages()
    .buildRequest()
    .get();

```