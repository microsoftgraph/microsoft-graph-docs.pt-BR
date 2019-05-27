---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 861d7eb3437c759ea5f9e517ce4d50764e768271
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34435540"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports.GetOneDriveActivityUserCounts('D7')
    .Request()
    .GetAsync();

```