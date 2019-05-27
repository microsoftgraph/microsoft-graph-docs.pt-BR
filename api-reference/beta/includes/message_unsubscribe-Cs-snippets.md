---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 35f5686cb351b5181c30b5d633b84e3c12404e74
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34443926"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Messages["{id}"]
    .Unsubscribe()
    .Request()
    .PostAsync();

```