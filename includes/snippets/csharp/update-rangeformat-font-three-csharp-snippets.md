---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b5a8a6b69e72b67cad356f248558a851645e9010
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36372682"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRangeFont = new WorkbookRangeFont
{
    Underline = "Single",
    Color = "#FFFFFF",
    Size = 26
};

await graphClient.Me.Drive.Items["{id}"].Workbook.Worksheets["Sheet1"]
    .Range("$C$1").Format.Font
    .Request()
    .UpdateAsync(workbookRangeFont);

```