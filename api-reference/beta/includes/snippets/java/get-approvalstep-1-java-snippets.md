---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 52875bdc0bd55cb56ace9a12f9ead0d639ec639a
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51209174"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ApprovalStepCollectionPage steps = graphClient.identityGovernance().entitlementManagement().accessPackageAssignmentApprovals("abd306ef-f7b2-4a10-9fd1-493454322489").steps()
    .buildRequest()
    .get();

```