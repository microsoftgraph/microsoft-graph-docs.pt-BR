---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a46e1ec5f4aca88a558912ca2781102577fbe0cc
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35891983"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRangeFill = new WorkbookRangeFill
{
    Color = "#00FF00"
};

await graphClient.Me.Drive.Items["{id}"].Workbook.Worksheets["{sheet-id}"]
    .Range('$B$1').Format.Fill
    .Request()
    .UpdateAsync(workbookRangeFill);

```