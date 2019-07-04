---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fd46820890955e4c75d704ef914505677fe7ecdf
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35533151"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRangeFill = new WorkbookRangeFill
{
    Color = "#FF0000"
};

await graphClient.Me.Drive.Items["{id}"].Workbook.Worksheets["Sheet1"].Range('$A$1').Format.Fill
    .Request()
    .UpdateAsync(workbookRangeFill);

```