---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e2b92ff44c85d032c15367457d320217146ac917
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50969500"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Boolean disableUserAccounts = true;

graphClient.domains("contoso.com")
    .forceDelete(DomainForceDeleteParameterSet
        .newBuilder()
        .withDisableUserAccounts(disableUserAccounts)
        .build())
    .buildRequest()
    .post();

```