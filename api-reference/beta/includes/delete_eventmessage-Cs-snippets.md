---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8395d7d42c9636d18f517679436f63d7ee8c8d16
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34438249"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Messages["{id}"]
    .Request()
    .DeleteAsync();

```