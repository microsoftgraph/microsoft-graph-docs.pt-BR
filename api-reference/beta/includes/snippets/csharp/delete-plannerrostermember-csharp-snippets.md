---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3926da821c56d09f2d0975dc80561f1a76937e7b
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50790488"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Planner.Rosters["{plannerRoster-id}"].Members["{plannerRosterMember-id}"]
    .Request()
    .DeleteAsync();

```