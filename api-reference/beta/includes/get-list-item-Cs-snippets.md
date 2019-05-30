---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 26d4810381be3bb443c6d93f12cb0231317ea8b6
ms.sourcegitcommit: c0df90d66cb2072848d4bb0bf730c47a601b99ce
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/29/2019
ms.locfileid: "34536544"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var queryOptions = new List<QueryOption>()
{
    new QueryOption("expand", "fields")
};

var listItem = await graphClient.Sites["{site-id}"].Lists["{list-id}"].Items["{item-id}"]
    .Request( queryOptions )
    .GetAsync();

```