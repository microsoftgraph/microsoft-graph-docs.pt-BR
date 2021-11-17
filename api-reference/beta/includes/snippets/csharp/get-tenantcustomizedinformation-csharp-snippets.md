---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 44b2628cc2b425fa97c0bf87015c0456f2c0ac3fc63b7f3bc262dcf451262703
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57156937"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tenantCustomizedInformation = await graphClient.TenantRelationships.ManagedTenants.TenantsCustomizedInformation["{managedTenants.tenantCustomizedInformation-id}"]
    .Request()
    .GetAsync();

```