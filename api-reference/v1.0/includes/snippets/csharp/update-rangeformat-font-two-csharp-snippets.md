---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b9a567112f98b0c265efd597e8d8976bf307c2b2
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35891972"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRangeFont = new WorkbookRangeFont
{
    Italic = true,
    Size = 26
};

await graphClient.Me.Drive.Items["{id}"].Workbook.Worksheets["{sheet-id}"]
    .Range('$B$1').Format.Font
    .Request()
    .UpdateAsync(workbookRangeFont);

```