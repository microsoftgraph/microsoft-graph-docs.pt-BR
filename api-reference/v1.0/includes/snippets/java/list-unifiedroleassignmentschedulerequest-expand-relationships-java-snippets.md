---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bbc87e6795456a1f15997be35e125be0576f6a39
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/05/2022
ms.locfileid: "65207244"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UnifiedRoleAssignmentScheduleRequestCollectionPage roleAssignmentScheduleRequests = graphClient.roleManagement().directory().roleAssignmentScheduleRequests()
    .buildRequest()
    .expand("roleDefinitionId")
    .select("principalId,action,roleDefinitionId")
    .get();

```