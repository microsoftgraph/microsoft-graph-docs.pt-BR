---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f94fe96b1c4730019fd64444cfb8ddc762759f53
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/15/2021
ms.locfileid: "53442596"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var managementActionTenantDeploymentStatus = await graphClient.TenantRelationships.ManagedTenants.ManagementActionTenantDeploymentStatuses["{managedTenants.managementActionTenantDeploymentStatus-id}"]
    .Request()
    .GetAsync();

```