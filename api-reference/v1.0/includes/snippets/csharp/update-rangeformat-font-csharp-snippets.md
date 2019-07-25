---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 13c314e95df8eb0cc0db5630a19f539e64d0b609
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35891980"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRangeFont = new WorkbookRangeFont
{
    Bold = true,
    Color = "#4B180E",
    Size = 26
};

await graphClient.Me.Drive.Items["{id}"].Workbook.Worksheets["{sheet-id}"]
    .Range('$A$1').Format.Font
    .Request()
    .UpdateAsync(workbookRangeFont);

```