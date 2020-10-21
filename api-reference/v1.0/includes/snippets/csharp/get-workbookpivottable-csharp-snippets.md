---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 57d3b50b60009360fbd281be76a7f204d6370099
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48620304"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookPivotTable = await graphClient.Me.Drive.Root.Workbook.Worksheets["{id}"].PivotTables["{id}"]
    .Request()
    .GetAsync();

```