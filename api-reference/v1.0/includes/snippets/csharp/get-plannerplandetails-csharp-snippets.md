---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3df35eb88f50778624018a21c91f34e4b36c5fa7
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48616356"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var plannerPlanDetails = await graphClient.Planner.Plans["{plan-id}"].Details
    .Request()
    .GetAsync();

```