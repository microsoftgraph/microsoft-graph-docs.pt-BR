---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7e5e51f16deaf4f3a6605212454616a2368574a205e0bb68a3750b6f557f9859
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57100998"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRangeFormat = new WorkbookRangeFormat
{
    ColumnWidth = 135,
    HorizontalAlignment = "Right",
    VerticalAlignment = "Top",
    RowHeight = 49,
    WrapText = false
};

await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Worksheets["{workbookWorksheet-id}"]
    .Range("$C$1").Format
    .Request()
    .UpdateAsync(workbookRangeFormat);

```