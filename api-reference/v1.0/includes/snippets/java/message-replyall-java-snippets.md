---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 166a150b20b84f10ea956386a1897b4a4dca1c37
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50983638"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String comment = "comment-value";

graphClient.me().messages("{id}")
    .replyAll(MessageReplyAllParameterSet
        .newBuilder()
        .withMessage(null)
        .withComment(comment)
        .build())
    .buildRequest()
    .post();

```