---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 83629738fcadcba26206e22aece568e4d8ddb8e9
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48613609"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var queryOptions = new List<QueryOption>()
{
    new QueryOption("search", "{query}")
};

var sites = await graphClient.Sites
    .Request( queryOptions )
    .GetAsync();

```