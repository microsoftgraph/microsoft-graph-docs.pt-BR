---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2c5fd76f4f40a1d025ed1c83f66271a871c06db2
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58258888"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var appManagementPolicy = new AppManagementPolicy
{
    IsEnabled = false
};

await graphClient.Policies.AppManagementPolicies["{appManagementPolicy-id}"]
    .Request()
    .UpdateAsync(appManagementPolicy);

```