---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c1b167466911c8954afa9beceb9984e6b6fe48a0
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34454156"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var sites = await graphClient.Sites
    .Request()
    .GetAsync();

```