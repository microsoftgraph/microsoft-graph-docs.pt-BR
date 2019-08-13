---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ac2b4d93e0ca45e8e325d1e54f3bd1c7e8e15ed3
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36324735"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRangeFont = new WorkbookRangeFont
{
    Bold = true,
    Color = "#4B180E",
    Size = 26
};

await graphClient.Me.Drive.Items["{id}"].Workbook.Worksheets["{sheet-id}"]
    .Range("$A$1").Format.Font
    .Request()
    .UpdateAsync(workbookRangeFont);

```