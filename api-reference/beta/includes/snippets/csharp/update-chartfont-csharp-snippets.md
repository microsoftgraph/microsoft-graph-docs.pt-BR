---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6526fbb2644ba1be4e5decad356daa34505e3ec6
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35475841"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookChartFont = new WorkbookChartFont
{
    Bold = true,
    Color = "color-value",
    Italic = true,
    Name = "name-value",
    Size = 99,
    Underline = "underline-value"
};

await graphClient.Me.Drive.Items["{id}"].Workbook.Worksheets["{id|name}"].Charts["{name}"].Axes.ValueAxis.Format.Font
    .Request()
    .UpdateAsync(workbookChartFont);

```