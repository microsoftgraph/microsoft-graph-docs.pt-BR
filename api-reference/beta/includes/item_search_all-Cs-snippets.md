---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9453d626b8d5e612ceb0acbd032ffdec5293dace
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34444493"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var search = await graphClient.Me.Drive.Search('{search-query}')
    .Request()
    .GetAsync();

```