---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bb6a05ee76e1ca5b0f3350d3ff65f315c247bf05
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "60980942"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tenantId = "String";

var tenantGroupId = "String";

var managementTemplateId = "String";

await graphClient.TenantRelationships.ManagedTenants.ManagementActions["{managedTenants.managementAction-id}"]
    .Apply(tenantId,tenantGroupId,managementTemplateId,null,null,null)
    .Request()
    .PostAsync();

```