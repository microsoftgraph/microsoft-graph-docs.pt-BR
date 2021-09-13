---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6c538a0ddae69b3f57f91fa86e28970aca83bad1cfe3c680627c4a6a77b8144c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215497"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<String> inputIdsList = new LinkedList<String>();
inputIdsList.add("{rest-formatted-id-1}");
inputIdsList.add("{rest-formatted-id-2}");

ExchangeIdFormat sourceIdType = ExchangeIdFormat.REST_ID;

ExchangeIdFormat targetIdType = ExchangeIdFormat.REST_IMMUTABLE_ENTRY_ID;

graphClient.me()
    .translateExchangeIds(UserTranslateExchangeIdsParameterSet
        .newBuilder()
        .withInputIds(inputIdsList)
        .withTargetIdType(targetIdType)
        .withSourceIdType(sourceIdType)
        .build())
    .buildRequest()
    .post();

```