---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 163ab4dad623cf48a1d5aad01e2cd51fdb834001
ms.sourcegitcommit: 42fdb068616222eb6b0813e93b33e830fc7eedc0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/17/2021
ms.locfileid: "50271881"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var plannerRoster = await graphClient.Planner.Rosters["6519868f-868f-6519-8f86-19658f861965"]
    .Request()
    .GetAsync();

```