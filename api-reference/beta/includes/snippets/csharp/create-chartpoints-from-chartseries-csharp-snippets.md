---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 171e3d1d437972ad32d64d59ecdf25bedc2ef6e700b85fb1137b58da40c3046e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57156264"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookChartPoint = new WorkbookChartPoint
{
};

await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Worksheets["{workbookWorksheet-id}"].Charts["{workbookChart-id}"].Series["{workbookChartSeries-id}"].Points
    .Request()
    .AddAsync(workbookChartPoint);

```