---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3746628347e22d4c4bb86cf57367dc04b212bb59
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34443996"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var destinationId = "deleteditems";

await graphClient.Me.Messages["AAMkADhAAATs28OAAA="]
    .Move(destinationId)
    .Request()
    .PostAsync();

```