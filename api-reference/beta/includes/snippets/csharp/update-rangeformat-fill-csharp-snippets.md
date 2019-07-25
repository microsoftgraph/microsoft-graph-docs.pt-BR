---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 471dece8f352cbdf2ce81c64cf8ea9b8ce5d6e13
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35874219"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRangeFill = new WorkbookRangeFill
{
    Color = "#FF0000"
};

await graphClient.Me.Drive.Items["{id}"].Workbook.Worksheets["Sheet1"]
    .Range('$A$1').Format.Fill
    .Request()
    .UpdateAsync(workbookRangeFill);

```