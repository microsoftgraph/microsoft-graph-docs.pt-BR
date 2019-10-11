---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 672688085b0864ca1daf88d38d45f122f36e4b66
ms.sourcegitcommit: 1585d55d3e7030b5fd1f7cfd5de8f9fb8202cd56
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/09/2019
ms.locfileid: "37428708"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var queryOptions = new List<QueryOption>()
{
    new QueryOption("format", "{format}")
};

var stream = await graphClient.Drive.Items["{item-id}"].Content
    .Request( queryOptions )
    .GetAsync();

```