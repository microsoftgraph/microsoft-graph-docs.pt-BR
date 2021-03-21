---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c1609e1056c55a44f6f504af1e4ca15955969542
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50981930"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String id = "id-value";

String groupId = "groupId-value";

graphClient.me().onenote().pages("{id}")
    .copyToSection(OnenotePageCopyToSectionParameterSet
        .newBuilder()
        .withId(id)
        .withGroupId(groupId)
        .withSiteCollectionId(null)
        .withSiteId(null)
        .build())
    .buildRequest()
    .post();

```