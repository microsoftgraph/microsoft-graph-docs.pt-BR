---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7cea20cb1472738691fd730d4bd0ebcf3a56aa62
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34462842"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var list = await graphClient.Sites["{site-id}"].Lists["{list-id}"]
    .Request()
    .GetAsync();

```