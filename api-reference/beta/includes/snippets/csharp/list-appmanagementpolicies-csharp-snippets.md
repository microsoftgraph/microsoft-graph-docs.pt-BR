---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f41c3c14750afe7bb49abf5c1af38ca2d28c8536
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58258920"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var appManagementPolicies = await graphClient.Policies.AppManagementPolicies
    .Request()
    .GetAsync();

```