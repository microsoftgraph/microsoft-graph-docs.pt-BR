---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 52b5e5e7a78c772f6d33ccd913135a954c8538b371f4dc132154bcdc992dc5a8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57272112"
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