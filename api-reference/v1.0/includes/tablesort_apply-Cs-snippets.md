---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a565d687e05cad30b71b17cde1f028ca56410548
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34435421"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var fields = new List<WorkbookSortField>()
{
    new WorkbookSortField
    {
        Key = 99,
        SortOn = "sortOn-value",
        Ascending = true,
        Color = "color-value",
        DataOption = "dataOption-value",
        Icon = new WorkbookIcon
        {
            Set = "set-value",
            Index = 99
        }
    }
};

var matchCase = true;

var method = "method-value";

await graphClient.Me.Drive.Items["{id}"].Workbook.Tables["{id|name}"].Sort
    .Apply(fields,matchCase,method)
    .Request()
    .PostAsync();

```