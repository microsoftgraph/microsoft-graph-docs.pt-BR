---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e21be8f4e25af2801077e83094ce5089f018fefe
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/15/2021
ms.locfileid: "53440908"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tenantGroupId = "String";

var tenantId = "String";

var managementActionId = "String";

var managementTemplateId = "String";

var status = "String";

await graphClient.TenantRelationships.ManagedTenants.ManagementActionTenantDeploymentStatuses
    .ChangeDeploymentStatus(tenantGroupId,tenantId,managementActionId,managementTemplateId,status)
    .Request()
    .PostAsync();

```