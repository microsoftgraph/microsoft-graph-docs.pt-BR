---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 528fe4d0195b56e54c7f3b07fec03be57ef701d7
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48620504"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookChartGridlines = await graphClient.Me.Drive.Items["{id}"].Workbook.Worksheets["{id|name}"].Charts["{name}"].Axes.ValueAxis.MinorGridlines
    .Request()
    .GetAsync();

```