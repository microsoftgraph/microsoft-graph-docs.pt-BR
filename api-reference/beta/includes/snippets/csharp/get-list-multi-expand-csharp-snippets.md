---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 727c044502df9ab5b0e74ff1f7fa3a6e47eabe81
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35499287"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var queryOptions = new List<QueryOption>()
{
    new QueryOption("select", "name,lastModifiedDateTime"),
    new QueryOption("expand", "columns(select=name,description),items(expand=fields(select=Name,Color,Quantity))")
};

var list = await graphClient.Sites["{site-id}"].Lists["{list-id}"]
    .Request( queryOptions )
    .GetAsync();

```