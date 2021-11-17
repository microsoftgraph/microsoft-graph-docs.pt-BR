---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ef2fac5b3aaeac03792538e131fa8481de181e50a958337b7402ef925f4bc80d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57326985"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var cloudPcOverview = await graphClient.TenantRelationships.ManagedTenants.CloudPcsOverview["{managedTenants.cloudPcOverview-id}"]
    .Request()
    .GetAsync();

```