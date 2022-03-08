---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e72f7790c7554730ca729c0df3d743fb69e258f3
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63336561"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var crossTenantAccessPolicy = await graphClient.Policies.CrossTenantAccessPolicy
    .Request()
    .GetAsync();

```