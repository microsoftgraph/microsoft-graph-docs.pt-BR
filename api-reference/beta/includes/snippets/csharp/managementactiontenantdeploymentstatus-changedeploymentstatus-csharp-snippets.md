---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b9db82069e13cb660ba0d2cd689531666d6ab6c8
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61022046"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tenantGroupId = "String";

var tenantId = "String";

var managementActionId = "String";

var managementTemplateId = "String";

var status = "String";

await graphClient.TenantRelationships.ManagedTenants.ManagementActionTenantDeploymentStatuses
    .ChangeDeploymentStatus(null,tenantGroupId,tenantId,managementActionId,managementTemplateId,status)
    .Request()
    .PostAsync();

```