---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8dfa8c70e2d79bfc5210078521c8540442c1101cf3fa2a06f8a455ff67c81584
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57214177"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String comment = "comment-value";

Boolean sendResponse = true;

graphClient.me().events("{id}")
    .accept(EventAcceptParameterSet
        .newBuilder()
        .withComment(comment)
        .withSendResponse(sendResponse)
        .build())
    .buildRequest()
    .post();

```