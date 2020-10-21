---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b22eb0997b2854af7c7d889c37585aee45967c39
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48608200"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var queryOptions = new List<QueryOption>()
{
    new QueryOption("select", "id,name,lastModifiedDateTime"),
    new QueryOption("expand", "columns(select=name,description),items(expand=fields(select=Name,Color,Quantity))")
};

var list = await graphClient.Sites["{site-id}"].Lists["{list-id}"]
    .Request( queryOptions )
    .GetAsync();

```