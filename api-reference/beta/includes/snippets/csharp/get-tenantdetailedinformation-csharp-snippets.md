---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e04adb17383b1d1a545f4b82156dcfc4fbc40579d8c6df6ad63bf713c0c8da49
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57157218"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tenantDetailedInformation = await graphClient.TenantRelationships.ManagedTenants.TenantsDetailedInformation["{managedTenants.tenantDetailedInformation-id}"]
    .Request()
    .GetAsync();

```