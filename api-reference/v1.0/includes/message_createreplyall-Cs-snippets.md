---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5757aa0abcca21238914310f22a2062bb3d42a86
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34455379"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Messages["{id}"]
    .CreateReplyAll()
    .Request()
    .PostAsync();

```