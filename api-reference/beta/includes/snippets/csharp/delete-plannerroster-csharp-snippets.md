---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a64f0e5d9f33047e8acfaff31451b4265e2d3dbf
ms.sourcegitcommit: 42fdb068616222eb6b0813e93b33e830fc7eedc0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/17/2021
ms.locfileid: "50271918"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Planner.Rosters["5ba84f7a-aa11-4a51-a298-9f2c7ec6bb38"]
    .Request()
    .DeleteAsync();

```