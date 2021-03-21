---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 01913f6be82426c748882113207e4df64a769cd3
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50978946"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

RejectReason reason = RejectReason.BUSY;

graphClient.communications().calls("57dab8b1-894c-409a-b240-bd8beae78896")
    .reject(CallRejectParameterSet
        .newBuilder()
        .withReason(reason)
        .withCallbackUri(null)
        .build())
    .buildRequest()
    .post();

```