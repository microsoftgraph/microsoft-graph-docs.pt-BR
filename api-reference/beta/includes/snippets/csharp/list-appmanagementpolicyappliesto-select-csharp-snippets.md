---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ae66c36a312c1c427928bfc1ecbf7720000c6d30
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58258962"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var appliesTo = await graphClient.Policies.AppManagementPolicies["{appManagementPolicy-id}"].AppliesTo
    .Request()
    .Select("id,appId,displayName,createdDateTime")
    .GetAsync();

```