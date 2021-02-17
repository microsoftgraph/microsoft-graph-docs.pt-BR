---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 51536b856bd3d723c7de542b9d2570530599399b
ms.sourcegitcommit: 42fdb068616222eb6b0813e93b33e830fc7eedc0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/17/2021
ms.locfileid: "50274719"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var plans = await graphClient.Groups["ebf3b108-5234-4e22-b93d-656d7dae5874"].Planner.Plans
    .Request()
    .GetAsync();

```