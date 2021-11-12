---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c44ec99080850364baf3c89ed4c1260bb773d5451756a7b0fc0331ca92d19223
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57272362"
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