---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 701ae598f700bb94fa82e30484a1b13f29462b83114a1574aea4407f94a8f772
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56900158"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookChartPoint = await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Worksheets["{workbookWorksheet-id}"].Charts["{workbookChart-id}"].Series["{workbookChartSeries-id}"].Points["{workbookChartPoint-id}"]
    .Request()
    .GetAsync();

```