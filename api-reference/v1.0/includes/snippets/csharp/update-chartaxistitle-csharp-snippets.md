---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 51f4ee31463669770147dc0f46af2153d055d515
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35492349"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookChartAxisTitle = new WorkbookChartAxisTitle
{
    Text = "text-value",
    Visible = true
};

await graphClient.Me.Drive.Items["{id}"].Workbook.Worksheets["{id|name}"].Charts["{name}"].Axes.ValueAxis.Title
    .Request()
    .UpdateAsync(workbookChartAxisTitle);

```