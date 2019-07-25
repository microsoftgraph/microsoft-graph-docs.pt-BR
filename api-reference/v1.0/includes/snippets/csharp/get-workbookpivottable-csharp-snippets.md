---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 57d3b50b60009360fbd281be76a7f204d6370099
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35711040"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookPivotTable = await graphClient.Me.Drive.Root.Workbook.Worksheets["{id}"].PivotTables["{id}"]
    .Request()
    .GetAsync();

```