---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1133eb04cad418ff106abfc4c238337eddc851bd
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34453212"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Drive.Root.Workbook.Worksheets["{id}"]
    .Range()
    .RowsAbove(count)
    .Request()
    .PostAsync();

```