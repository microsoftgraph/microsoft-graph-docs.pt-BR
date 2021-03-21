---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9db73673f3d181ab661824201dc2439edd0bd55b
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50968647"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String destinationId = "deleteditems";

graphClient.me().messages("AAMkADhAAATs28OAAA=")
    .move(MessageMoveParameterSet
        .newBuilder()
        .withDestinationId(destinationId)
        .build())
    .buildRequest()
    .post();

```