---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a6187c0d78ba5b7abb601b3c8fbabcbfda75c1d5
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48605611"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookWorksheet = new WorkbookWorksheet
{
    Position = 99,
    Name = "name-value",
    Visibility = "visibility-value"
};

await graphClient.Me.Drive.Items["{id}"].Workbook.Worksheets["{id|name}"]
    .Request()
    .UpdateAsync(workbookWorksheet);

```