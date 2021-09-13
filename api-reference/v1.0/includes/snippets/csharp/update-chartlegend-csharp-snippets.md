---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1b1b53384973e0e04599fad0d42082ba1872a3aea8ea9670271ab0a7a098f6bf
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215011"
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