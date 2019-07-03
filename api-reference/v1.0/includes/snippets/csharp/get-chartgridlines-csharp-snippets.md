---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 528fe4d0195b56e54c7f3b07fec03be57ef701d7
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35466111"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookChartGridlines = await graphClient.Me.Drive.Items["{id}"].Workbook.Worksheets["{id|name}"].Charts["{name}"].Axes.ValueAxis.MinorGridlines
    .Request()
    .GetAsync();

```