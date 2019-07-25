---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b87625df1219cb3ba64972c0215488476b916774
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35708442"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookChartAxis = await graphClient.Me.Drive.Items["{id}"].Workbook.Worksheets["{id|name}"].Charts["{name}"].Axes.ValueAxis
    .Request()
    .GetAsync();

```