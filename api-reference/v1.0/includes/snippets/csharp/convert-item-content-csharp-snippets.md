---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 78e0dea1220686cb1bc2cbc065586784961c586b
ms.sourcegitcommit: 1585d55d3e7030b5fd1f7cfd5de8f9fb8202cd56
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/09/2019
ms.locfileid: "37428753"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var queryOptions = new List<QueryOption>()
{
    new QueryOption("format", "{format}")
};

var stream = await graphClient.Me.Drive.Items["{item-id}"].Content
    .Request( queryOptions )
    .GetAsync();

```