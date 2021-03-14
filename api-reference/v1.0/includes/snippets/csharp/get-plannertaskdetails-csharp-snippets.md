---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 734de2abb51ea3673536da813cf5d64ec752b382
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50787292"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var plannerTaskDetails = await graphClient.Planner.Tasks["{plannerTask-id}"].Details
    .Request()
    .GetAsync();

```