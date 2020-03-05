---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f9fd20a6c9857ce384d58870e8b5946dd988541d
ms.sourcegitcommit: 2f78ac96a9b0462626a242429055ef824590bd3f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2020
ms.locfileid: "41475515"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var {id} = await graphClient.Policies["activityBasedTimeoutPolicies"].{id}
    .Request()
    .GetAsync();

```