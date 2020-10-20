---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 10205edf6394db9750288ed4a628b6eacd151854
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48604846"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRangeBorder = new WorkbookRangeBorder
{
    Id = "id-value",
    Color = "color-value",
    Style = "style-value",
    SideIndex = "sideIndex-value",
    Weight = "weight-value"
};

await graphClient.Me.Drive.Items["{id}"].Workbook.Names["{name}"]
    .Range().Format.Borders
    .Request()
    .AddAsync(workbookRangeBorder);

```