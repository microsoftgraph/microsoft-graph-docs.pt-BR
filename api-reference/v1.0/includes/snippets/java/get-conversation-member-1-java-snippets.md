---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8209fb9af288ef9f63c2d5fef78dbf16a012f259
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51202378"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ConversationMember conversationMember = graphClient.chats("19:cf66807577b149cca1b7af0c32eec122@thread.v2").members("141c574c-dd90-4131-b173-baf4bb0e894e")
    .buildRequest()
    .get();

```