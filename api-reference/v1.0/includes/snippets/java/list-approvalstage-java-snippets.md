---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cba9ecdac3fda6678b4399c60cc13db7d8c25c3e
ms.sourcegitcommit: 0bcc0a93f37db6013be40dc8d36717aeeeef7fb6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/16/2022
ms.locfileid: "63515804"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ApprovalStageCollectionPage stages = graphClient.identityGovernance().entitlementManagement().accessPackageAssignmentApprovals("abd306ef-f7b2-4a10-9fd1-493454322489").stages()
    .buildRequest()
    .get();

```