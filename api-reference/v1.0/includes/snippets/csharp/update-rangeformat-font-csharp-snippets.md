---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1a3265b9ac5e6745c08e1e96a91cc713004f0ce6
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35466001"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRangeFont = new WorkbookRangeFont
{
    Bold = true,
    Color = "#4B180E",
    Size = 26
};

await graphClient.Me.Drive.Items["{id}"].Workbook.Worksheets["{sheet-id}"].Range('$A$1').Format.Font
    .Request()
    .UpdateAsync(workbookRangeFont);

```