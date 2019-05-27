---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9126fec0749cf8b3dd143b11d2b63b59596d3833
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34473558"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var buckets = await graphClient.Planner.Plans["2txjA-BMZEq-bKi6Wfj5aGQAB1OJ"].Buckets
    .Request()
    .GetAsync();

```