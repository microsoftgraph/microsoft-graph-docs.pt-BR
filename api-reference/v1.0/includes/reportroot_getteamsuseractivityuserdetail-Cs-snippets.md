---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a567b51f3ca35fcaf1ae99a50bad85c273d1e088
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34434798"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports.GetTeamsUserActivityUserDetail('D7')
    .Request()
    .GetAsync();

```