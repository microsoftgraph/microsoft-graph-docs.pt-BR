---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 21bc7d8d6c3eef9eaa4843f902a7728f0465d8b7
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34461640"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRangeFont = new WorkbookRangeFont
{
    Italic = true,
    Size = 26
};

await graphClient.Me.Drive.Items["{id}"].Workbook.Worksheets["Sheet1"].Range('$B$1').Format.Font
    .Request()
    .UpdateAsync(workbookRangeFont);

```