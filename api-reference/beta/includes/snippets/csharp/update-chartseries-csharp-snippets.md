---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 23ec53bdc5b18bb28dd434064892da3b8b02723c
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48609328"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookChartSeries = new WorkbookChartSeries
{
    Name = "name-value"
};

await graphClient.Me.Drive.Items["{id}"].Workbook.Worksheets["{id|name}"].Charts["{name}"].Series["{undefined}"]
    .Request()
    .UpdateAsync(workbookChartSeries);

```