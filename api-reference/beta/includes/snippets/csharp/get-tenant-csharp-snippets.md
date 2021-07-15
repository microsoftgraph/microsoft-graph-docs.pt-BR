---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7b2a78cff3cf611c605ee23fd855cc08ae586fc3
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/15/2021
ms.locfileid: "53442466"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tenant = await graphClient.TenantRelationships.ManagedTenants.Tenants["{managedTenants.tenant-id}"]
    .Request()
    .GetAsync();

```