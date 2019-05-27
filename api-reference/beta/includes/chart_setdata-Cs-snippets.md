---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 225dc419576d2658567bea450d2aa070d0b2c515
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34474839"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var sourceData = "sourceData-value";

var seriesBy = "seriesBy-value";

await graphClient.Me.Drive.Items["{id}"].Workbook.Worksheets["{id|name}"].Charts["{name}"]
    .SetData(sourceData,seriesBy)
    .Request()
    .PostAsync();

```