---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 431fab54e6447c59fbc88fd888e9576ccdfcb3b4
ms.sourcegitcommit: 0bcc0a93f37db6013be40dc8d36717aeeeef7fb6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/16/2022
ms.locfileid: "63515792"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ApprovalFilterByCurrentUserCollectionPage filterByCurrentUser = graphClient.identityGovernance().entitlementManagement().accessPackageAssignmentApprovals()
    .filterByCurrentUser(ApprovalFilterByCurrentUserParameterSet
        .newBuilder()
        .withOn('approver')
        .build())
    .buildRequest()
    .get();

```