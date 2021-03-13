---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 51b94a13e774ebcea95f710c0148a8f7b18c80c2
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50786168"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var plannerBucket = await graphClient.Planner.Buckets["{plannerBucket-id}"]
    .Request()
    .GetAsync();

```