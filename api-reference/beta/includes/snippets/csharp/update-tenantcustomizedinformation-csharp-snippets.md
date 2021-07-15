---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e051d45a71ed53cc8984ac563004652976892edb
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/15/2021
ms.locfileid: "53441793"
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