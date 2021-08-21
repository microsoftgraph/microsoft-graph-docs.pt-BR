---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c4eee0208f876394cad17eac34bfa45cfa19b6e56ea64a80b2a5f5754d63a6f1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57160064"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

RbacApplicationRoleScheduleInstancesCollectionPage roleScheduleInstances = graphClient.roleManagement().directory()
    .roleScheduleInstances(RbacApplicationRoleScheduleInstancesParameterSet
        .newBuilder()
        .withDirectoryScopeId("parameterValue")
        .withAppScopeId("parameterValue")
        .withPrincipalId("parameterValue")
        .withRoleDefinitionId("parameterValue")
        .build())
    .buildRequest()
    .get();

```