---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 03dd31ac978b0c1249e39558550c2ed3d8a8a617d89c73cbf4cc32ff5eeff58e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57275476"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tenantCustomizedInformation = new Microsoft.Graph.ManagedTenants.TenantCustomizedInformation
{
    TenantId = "String",
    Contacts = new List<Microsoft.Graph.ManagedTenants.TenantContactInformation>()
    {
        new TenantContactInformation
        {
        }
    },
    Website = "String"
};

await graphClient.TenantRelationships.ManagedTenants.TenantsCustomizedInformation["{managedTenants.tenantCustomizedInformation-id}"]
    .Request()
    .UpdateAsync(tenantCustomizedInformation);

```