---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 839120b44d84ec2279d2116510cef1898d791a60
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35874232"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRangeFill = new WorkbookRangeFill
{
    Color = "#00FF00"
};

await graphClient.Me.Drive.Items["{id}"].Workbook.Worksheets["Sheet1"]
    .Range('$B$1').Format.Fill
    .Request()
    .UpdateAsync(workbookRangeFill);

```