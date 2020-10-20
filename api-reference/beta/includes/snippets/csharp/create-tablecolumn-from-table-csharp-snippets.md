---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a3a29ec51ef2212fc52175fcf9a8ff8f771100f5
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48611378"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookTableColumn = new WorkbookTableColumn
{
    Id = 99,
    Name = "name-value",
    Index = 99,
    Values = "values-value"
};

await graphClient.Me.Drive.Items["{id}"].Workbook.Tables["{id|name}"].Columns
    .Request()
    .AddAsync(workbookTableColumn);

```