---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2727e8ef4b6ff362d7c4e032161bf66bdbc4f06e
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50785097"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var plannerRosterMember = new PlannerRosterMember
{
    UserId = "String"
};

await graphClient.Planner.Rosters["{plannerRoster-id}"].Members
    .Request()
    .AddAsync(plannerRosterMember);

```