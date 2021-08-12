---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 75b4ef402ff4bd5ab8fd59f48f3b708ecea87454f48fbc9e581920349db3f76c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54237685"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRangeFormat = new WorkbookRangeFormat
{
    ColumnWidth = 135,
    VerticalAlignment = "Top",
    RowHeight = 49,
    WrapText = false
};

await graphClient.Me.Drive.Items["{id}"].Workbook.Worksheets["Sheet1"]
    .Range("$A$1").Format
    .Request()
    .UpdateAsync(workbookRangeFormat);

```