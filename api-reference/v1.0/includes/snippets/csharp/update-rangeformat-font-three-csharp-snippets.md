---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cb89f3d4668740eb7a906aa888728df4a8397d84
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36324745"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRangeFont = new WorkbookRangeFont
{
    Underline = "Single",
    Color = "#FFFFFF",
    Size = 26
};

await graphClient.Me.Drive.Items["{id}"].Workbook.Worksheets["{sheet-id}"]
    .Range("$C$1").Format.Font
    .Request()
    .UpdateAsync(workbookRangeFont);

```