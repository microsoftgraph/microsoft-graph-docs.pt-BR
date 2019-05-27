---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5b70d39ed880bc94c6bd81fc363cc386b0c7b91f
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34436751"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var Comment = "Cancelling for this week due to all hands";

await graphClient.Me.Events["{id}"]
    .Cancel(comment)
    .Request()
    .PostAsync();

```