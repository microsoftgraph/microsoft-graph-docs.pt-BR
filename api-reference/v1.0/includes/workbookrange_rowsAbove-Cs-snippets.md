---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 49d73037ec5ae6a0bc2f58d14fcfc633488ddf54
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34450535"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Drive.Root.Workbook.Worksheets["{id}"]
    .Range()
    .RowsAbove(count)
    .Request()
    .PostAsync();

```