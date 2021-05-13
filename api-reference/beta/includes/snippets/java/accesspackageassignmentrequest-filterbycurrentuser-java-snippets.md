---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 191cb6b1a6ccce935baeaf7624de5bac7ca0e1f0
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2021
ms.locfileid: "52473939"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessPackageFilterByCurrentUserCollectionPage filterByCurrentUser = graphClient.identityGovernance().entitlementManagement().accessPackages()
    .filterByCurrentUser(AccessPackageFilterByCurrentUserParameterSet
        .newBuilder()
        .withOn('allowedRequestor')
        .build())
    .buildRequest()
    .get();

```