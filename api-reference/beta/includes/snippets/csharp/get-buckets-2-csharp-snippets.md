---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 10992f84ef015eff6d32f2597e08a12102ed5a86
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50945908"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var buckets = await graphClient.Planner.Plans["{plannerPlan-id}"].Buckets
    .Request()
    .GetAsync();

```