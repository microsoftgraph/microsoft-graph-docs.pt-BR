---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 03184e5ffd23711f8a557e17f674dffc6a2bfdd7
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/15/2021
ms.locfileid: "53441797"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tenantId = "String";

await graphClient.TenantRelationships.ManagedTenants.TenantGroups
    .TenantSearch(tenantId)
    .Request()
    .PostAsync();

```