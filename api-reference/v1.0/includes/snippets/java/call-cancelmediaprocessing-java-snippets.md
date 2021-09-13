---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0427a91ace8c9664e703a6aebf6adcd8d21b5b016108ffa63269818e7b5ddc98
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57103083"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String clientContext = "clientContext-value";

graphClient.communications().calls("{id}")
    .cancelMediaProcessing(CallCancelMediaProcessingParameterSet
        .newBuilder()
        .withClientContext(clientContext)
        .build())
    .buildRequest()
    .post();

```