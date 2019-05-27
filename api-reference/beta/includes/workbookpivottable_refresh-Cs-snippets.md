---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 51aa7df113adac6a19963b2e2aed4f233725dcc5
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34456551"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Drive.Root.Workbook.Worksheets["{id}"].PivotTables["{id}"]
    .Refresh()
    .Request()
    .PostAsync();

```