---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 25f269fcecea906818aff9c50e8988229d706840
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61022045"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String tenantGroupId = "String";

String tenantId = "String";

String managementActionId = "String";

String managementTemplateId = "String";

String status = "String";

graphClient.tenantRelationships().managedTenants().managementActionTenantDeploymentStatuses()
    .changeDeploymentStatus(ManagementActionTenantDeploymentStatusChangeDeploymentStatusParameterSet
        .newBuilder()
        .withTenantGroupId(tenantGroupId)
        .withTenantId(tenantId)
        .withManagementActionId(managementActionId)
        .withManagementTemplateId(managementTemplateId)
        .withManagementTemplateVersion(null)
        .withStatus(status)
        .build())
    .buildRequest()
    .post();

```