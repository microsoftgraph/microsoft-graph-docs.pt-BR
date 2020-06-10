---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a42711849bd3b5b3777cd52cb2e23551f8bd752c
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/10/2020
ms.locfileid: "44685081"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookChartAxis = new WorkbookChartAxis
{
    MajorUnit = JToken.Parse("{}"),
    Maximum = JToken.Parse("{}"),
    Minimum = JToken.Parse("{}")
};

await graphClient.Me.Drive.Items["{id}"].Workbook.Worksheets["{id|name}"].Charts["{name}"].Axes.ValueAxis
    .Request()
    .UpdateAsync(workbookChartAxis);

```