---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e77b96f2b905782823870a2eb26e87c9ddce5304
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34461696"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRangeFill = new WorkbookRangeFill
{
    Color = "#00FF00"
};

await graphClient.Me.Drive.Items["{id}"].Workbook.Worksheets["Sheet1"].Range('$B$1').Format.Fill
    .Request()
    .UpdateAsync(workbookRangeFill);

```