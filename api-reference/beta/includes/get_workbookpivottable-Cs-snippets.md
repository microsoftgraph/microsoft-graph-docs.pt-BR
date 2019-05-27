---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fb4fd2977a1489975a053f29b201a26bc9a40525
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34445109"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookPivotTable = await graphClient.Drive.Root.Workbook.Worksheets["{id}"].PivotTables["{id}"]
    .Request()
    .GetAsync();

```