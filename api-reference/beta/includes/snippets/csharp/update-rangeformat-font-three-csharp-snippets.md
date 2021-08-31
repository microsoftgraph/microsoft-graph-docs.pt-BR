---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 29b4e73c53f0f114694a9aa636eb5b962273443a14fd150db628a8b5e10ba1bd
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57102247"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRangeFont = new WorkbookRangeFont
{
    Underline = "Single",
    Color = "#FFFFFF",
    Size = 26
};

await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Worksheets["{workbookWorksheet-id}"]
    .Range("$C$1").Format.Font
    .Request()
    .UpdateAsync(workbookRangeFont);

```