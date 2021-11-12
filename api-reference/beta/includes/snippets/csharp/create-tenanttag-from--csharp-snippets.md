---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6a6c9076312b5d0a0f9aca82ace54dd2dd9058575cd57fb5f988195862baaa43
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57099657"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tenantTag = new Microsoft.Graph.ManagedTenants.TenantTag
{
    DisplayName = "Support",
    Description = "Tenants that have purchased extended support"
};

await graphClient.TenantRelationships.ManagedTenants.TenantTags
    .Request()
    .AddAsync(tenantTag);

```