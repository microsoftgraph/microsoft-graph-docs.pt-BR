---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 459800448ff7fced90890bf0b6951683f4dedcf3
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35463371"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var queryOptions = new List<QueryOption>()
{
    new QueryOption("expand", "fields(select=Name,Color,Quantity)")
};

var items = await graphClient.Sites["{site-id}"].Lists["{list-id}"].Items
    .Request( queryOptions )
    .GetAsync();

```