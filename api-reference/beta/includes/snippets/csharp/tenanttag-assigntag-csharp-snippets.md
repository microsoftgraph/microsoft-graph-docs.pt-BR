---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7796f59a0c9287a6c00bc9395a87a410e75c121d042dcd9d77e81a268f95f230
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57100448"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tenantIds = new List<String>()
{
    "String"
};

await graphClient.TenantRelationships.ManagedTenants.TenantTags["{managedTenants.tenantTag-id}"]
    .AssignTag(tenantIds)
    .Request()
    .PostAsync();

```