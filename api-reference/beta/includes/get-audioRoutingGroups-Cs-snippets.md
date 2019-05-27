---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 141f966b551e1cc9c821c73b525fdbb423b2fb08
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34436408"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var audioRoutingGroups = await graphClient.App.Calls["{id}"].AudioRoutingGroups
    .Request()
    .GetAsync();

```