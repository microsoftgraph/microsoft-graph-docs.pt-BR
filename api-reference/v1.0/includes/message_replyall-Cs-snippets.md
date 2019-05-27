---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 14c5c1e6d7860a659ffbbf99e2c0f5459e27cbb1
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34461486"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var comment = "comment-value";

await graphClient.Me.Messages["{id}"]
    .ReplyAll(comment)
    .Request()
    .PostAsync();

```