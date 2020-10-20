---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 749ecae73c2aeba28b2234705fa4a153b034721c
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48604916"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookChart = new WorkbookChart
{
    Height = 99,
    Left = 99
};

await graphClient.Me.Drive.Items["{id}"].Workbook.Worksheets["{id|name}"].Charts["{name}"]
    .Request()
    .UpdateAsync(workbookChart);

```