---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9777e24d2d45e6b613ed81b94259fc8c6217b538
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35740405"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var pivotTables = await graphClient.Me.Drive.Root.Workbook.Worksheets["{id}"].PivotTables
    .Request()
    .GetAsync();

```