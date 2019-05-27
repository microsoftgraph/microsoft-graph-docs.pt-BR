---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0bd03f454d34c55871ba94a41c79d172ea77f3be
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34461549"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var comment = "comment-value";

await graphClient.Me.Messages["{id}"]
    .Reply(comment)
    .Request()
    .PostAsync();

```