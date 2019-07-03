---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0438d26738016be4fe069efc547e3a8707b7746d
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35498962"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var criteria = new WorkbookFilterCriteria
{
    Criterion1 = "criterion1-value",
    Criterion2 = "criterion2-value",
    Color = "color-value",
    Operator = new String
    {
    },
    Icon = new WorkbookIcon
    {
        Set = "set-value",
        Index = 99
    },
    DynamicCriteria = "dynamicCriteria-value",
    Values = new Json
    {
    },
    FilterOn = "filterOn-value"
};

await graphClient.Me.Drive.Items["{id}"].Workbook.Tables["{id|name}"].Columns["{id|name}"].Filter
    .Apply(criteria)
    .Request()
    .PostAsync();

```