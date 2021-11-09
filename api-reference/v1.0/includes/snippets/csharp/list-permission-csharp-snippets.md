---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 83629738fcadcba26206e22aece568e4d8ddb8e9
ms.sourcegitcommit: ddeee0eec277df06d9e635e5b5c257d14c856273
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/04/2021
ms.locfileid: "60783002"
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