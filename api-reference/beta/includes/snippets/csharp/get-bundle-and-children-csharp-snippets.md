---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 435efebe762d63fdb283cabef8659bc5b7ddadba86d5da0ab700618081746946
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57102172"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var queryOptions = new List<QueryOption>()
{
    new QueryOption("expand", "children")
};

var driveItem = await graphClient.Drive.Items["{driveItem-id}"]
    .Request( queryOptions )
    .GetAsync();

```