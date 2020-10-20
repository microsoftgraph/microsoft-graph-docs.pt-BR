---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9126fec0749cf8b3dd143b11d2b63b59596d3833
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48613400"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var buckets = await graphClient.Planner.Plans["2txjA-BMZEq-bKi6Wfj5aGQAB1OJ"].Buckets
    .Request()
    .GetAsync();

```