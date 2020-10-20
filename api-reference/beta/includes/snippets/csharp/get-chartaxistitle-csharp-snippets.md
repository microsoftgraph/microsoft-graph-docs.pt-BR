---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 21aca384bfecdf71328cfbae52e38e6e08a00505
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48617455"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookChartAxisTitle = await graphClient.Me.Drive.Items["{id}"].Workbook.Worksheets["{id|name}"].Charts["{name}"].Axes.ValueAxis.Title
    .Request()
    .GetAsync();

```