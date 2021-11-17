---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fe3a6e2fe3834174bf47e38ce933131c1b84588f3a6f7a05764902dabe14a334
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57272559"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tenantsCustomizedInformation = await graphClient.TenantRelationships.ManagedTenants.TenantsCustomizedInformation
    .Request()
    .GetAsync();

```