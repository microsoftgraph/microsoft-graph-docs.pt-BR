---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3df35eb88f50778624018a21c91f34e4b36c5fa7
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35734324"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var plannerPlanDetails = await graphClient.Planner.Plans["{plan-id}"].Details
    .Request()
    .GetAsync();

```