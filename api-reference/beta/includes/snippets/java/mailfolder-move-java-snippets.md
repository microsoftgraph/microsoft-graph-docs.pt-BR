---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: db83537da23d0e64aa77e80c571528dfe94a2050fff3fb25f3aca9ed43dac526
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57102504"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String destinationId = "destinationId-value";

graphClient.me().mailFolders("{id}")
    .move(MailFolderMoveParameterSet
        .newBuilder()
        .withDestinationId(destinationId)
        .build())
    .buildRequest()
    .post();

```