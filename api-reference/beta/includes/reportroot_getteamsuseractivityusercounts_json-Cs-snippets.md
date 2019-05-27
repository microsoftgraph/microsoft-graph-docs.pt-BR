---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a95443822db21a5b49f4b572c00ba01808a6c6bc
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34462912"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getTeamsUserActivityUserCounts = await graphClient.Reports.GetTeamsUserActivityUserCounts('D7')
    .Request()
    .GetAsync();

```