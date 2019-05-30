---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 49914b3bfbaf0cb9c492a50d5efb447e27ef49fe
ms.sourcegitcommit: c0df90d66cb2072848d4bb0bf730c47a601b99ce
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/29/2019
ms.locfileid: "34537396"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var queryOptions = new List<QueryOption>()
{
    new QueryOption("select", "c300x400_Crop")
};

var thumbnails = await graphClient.Me.Drive.Items["{item-id}"].Thumbnails
    .Request( queryOptions )
    .GetAsync();

```