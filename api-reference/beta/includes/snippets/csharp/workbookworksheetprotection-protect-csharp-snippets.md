---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 650f253ed5663d1a117c0878744c33160cf5dba7
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48615613"
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

await graphClient.Me.Drive.Items["{id}"].Workbook.Worksheets["{id|name}"].Protection
    .Protect(options)
    .Request()
    .PostAsync();

```