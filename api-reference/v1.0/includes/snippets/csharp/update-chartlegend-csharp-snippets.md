---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c7b42e093c06caec749cb0ca080c060812935637
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50806055"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookChartLegend = new WorkbookChartLegend
{
    Visible = true,
    Position = "position-value",
    Overlay = true
};

await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Worksheets["{workbookWorksheet-id}"].Charts["{workbookChart-id}"].Legend
    .Request()
    .UpdateAsync(workbookChartLegend);

```