---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 48f73a993525de9e85e60525b6324948ced2cc50
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48617037"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookChart = new WorkbookChart
{
    Id = "id-value",
    Height = 99,
    Left = 99
};

await graphClient.Me.Drive.Items["{id}"].Workbook.Worksheets["{id|name}"].Charts
    .Request()
    .AddAsync(workbookChart);

```