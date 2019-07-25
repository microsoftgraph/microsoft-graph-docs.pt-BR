---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 55f5d3fbafc941d0b5093ea1fe0b325338c37cf8
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35891985"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRangeFill = new WorkbookRangeFill
{
    Color = "#0000FF"
};

await graphClient.Me.Drive.Items["{id}"].Workbook.Worksheets["{sheet-id}"]
    .Range('$C$1').Format.Fill
    .Request()
    .UpdateAsync(workbookRangeFill);

```