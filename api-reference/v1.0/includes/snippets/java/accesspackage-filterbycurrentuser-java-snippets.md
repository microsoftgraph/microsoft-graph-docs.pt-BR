---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 191cb6b1a6ccce935baeaf7624de5bac7ca0e1f0
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2021
ms.locfileid: "61338013"
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