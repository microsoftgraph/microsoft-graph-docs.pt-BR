---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bf01f749ab5c78914b5402a13206384b391b41192948011a4f5cf9808173455b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57159042"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var options = new WorkbookWorksheetProtectionOptions
{
    AllowFormatCells = true,
    AllowFormatColumns = true,
    AllowFormatRows = true,
    AllowInsertColumns = true,
    AllowInsertRows = true,
    AllowInsertHyperlinks = true,
    AllowDeleteColumns = true,
    AllowDeleteRows = true,
    AllowSort = true,
    AllowAutoFilter = true,
    AllowPivotTables = true
};

await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Worksheets["{workbookWorksheet-id}"].Protection
    .Protect(options)
    .Request()
    .PostAsync();

```