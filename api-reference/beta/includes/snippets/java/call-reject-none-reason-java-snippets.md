---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8cb15eef3b29f3ca1e8f0dfc87cec48b5aed165c505a042f65bcfbb91a43a4ae
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57099419"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

RejectReason reason = RejectReason.NONE;

graphClient.communications().calls("57dab8b1-894c-409a-b240-bd8beae78896")
    .reject(CallRejectParameterSet
        .newBuilder()
        .withReason(reason)
        .withCallbackUri(null)
        .build())
    .buildRequest()
    .post();

```