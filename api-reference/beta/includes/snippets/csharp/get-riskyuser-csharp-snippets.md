---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e96555ead3e331fb109fece402019e58c0044933
ms.sourcegitcommit: 64d27a0e3dcccc9d857e62aace4153e5d98fb3d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/03/2021
ms.locfileid: "60730491"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var response = await graphClient.TenantRelationships.ManagedTenants.RiskyUsers["{UNKNOWN-id}"]
    .Request()
    .GetAsync();

```