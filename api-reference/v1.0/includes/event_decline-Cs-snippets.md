---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b51f7858ee54c5c7103444f112a56fa3b552375d
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34457828"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var comment = "comment-value";

var sendResponse = true;

await graphClient.Me.Events["{id}"]
    .Decline(comment,sendResponse)
    .Request()
    .PostAsync();

```