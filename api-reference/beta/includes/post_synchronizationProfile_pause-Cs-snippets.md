---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 798b04e49bd013620af376f196023edbbbce9e81
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34443289"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Education.SynchronizationProfiles["{id}"]
    .Pause()
    .Request()
    .PostAsync();

```