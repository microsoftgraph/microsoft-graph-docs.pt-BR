---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ded579acf29f1824a5c78c55b9c0d5751c917de7
ms.sourcegitcommit: 9b8abc940a68dac6ee5da105ca29800cb59775f6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/25/2021
ms.locfileid: "58514334"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UnifiedRoleAssignmentScheduleFilterByCurrentUserCollectionPage filterByCurrentUser = graphClient.roleManagement().directory().roleAssignmentSchedules()
    .filterByCurrentUser(UnifiedRoleAssignmentScheduleFilterByCurrentUserParameterSet
        .newBuilder()
        .withOn('principal')
        .build())
    .buildRequest()
    .get();

```