---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e62cd3e02f128f998a75b9e8dac5ecd92780283a
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34459133"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Events["{id}"]
    .Request()
    .DeleteAsync();

```