---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1b7d1b3abae89c62b9967d8bc7fceca07429556b
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2021
ms.locfileid: "61337141"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessPackageAssignmentRequestFilterByCurrentUserCollectionPage filterByCurrentUser = graphClient.identityGovernance().entitlementManagement().assignmentRequests()
    .filterByCurrentUser(AccessPackageAssignmentRequestFilterByCurrentUserParameterSet
        .newBuilder()
        .withOn('target')
        .build())
    .buildRequest()
    .get();

```