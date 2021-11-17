---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d67fd980528de2980e4ffcde7877288345fa5b3e9bbb689d2afe87eb063e2b99
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56899947"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tenants = await graphClient.TenantRelationships.ManagedTenants.Tenants
    .Request()
    .GetAsync();

```