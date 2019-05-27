---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c37f87c5ee87c32ea44f4fb5977f9079f4863ce8
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34450025"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var index = 3;

var values = new List<Json>()
{
    new Json
    {
    }
};

await graphClient.Me.Drive.Items["{id}"].Workbook.Tables["{id|name}"].Columns
    .Add(index,values,name)
    .Request()
    .PostAsync();

```