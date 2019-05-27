---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7611f3f6de81fd57479c8e7044a5665e876dc097
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34456558"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Drive.Root.Workbook.Worksheets["{id}"].PivotTables
    .RefreshAll()
    .Request()
    .PostAsync();

```