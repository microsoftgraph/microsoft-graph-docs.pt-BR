---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 65cf70a7b0b2277e217ba9857f0806c2f8c8822b
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34451879"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var color = "color-value";

await graphClient.Me.Drive.Items["{id}"].Workbook.Worksheets["{id|name}"].Charts["{name}"].Format.Fill
    .SetSolidColor(color)
    .Request()
    .PostAsync();

```