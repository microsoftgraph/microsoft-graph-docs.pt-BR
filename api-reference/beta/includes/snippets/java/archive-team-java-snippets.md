---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ad0fa61e9916d2e6f02dd2a1584293a8cf50adf1
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50981040"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.teams("{id}")
    .archive(TeamArchiveParameterSet
        .newBuilder()
        .withShouldSetSpoSiteReadOnlyForMembers(null)
        .build())
    .buildRequest()
    .post();

```