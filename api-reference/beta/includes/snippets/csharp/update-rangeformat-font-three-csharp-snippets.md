---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a74801019326893160bdfabd8422832bf6bc6996
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35874236"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRangeFont = new WorkbookRangeFont
{
    Underline = "Single",
    Color = "#FFFFFF",
    Size = 26
};

await graphClient.Me.Drive.Items["{id}"].Workbook.Worksheets["Sheet1"]
    .Range('$C$1').Format.Font
    .Request()
    .UpdateAsync(workbookRangeFont);

```