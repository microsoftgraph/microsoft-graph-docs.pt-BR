---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e42878f25206231dfcde1964f76a25ac9dde0115
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50979074"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String clientContext = "clientContext-value";

graphClient.communications().calls("57dab8b1-894c-409a-b240-bd8beae78896")
    .unmute(CallUnmuteParameterSet
        .newBuilder()
        .withClientContext(clientContext)
        .build())
    .buildRequest()
    .post();

```