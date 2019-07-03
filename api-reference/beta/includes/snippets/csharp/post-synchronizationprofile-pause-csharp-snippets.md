---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 798b04e49bd013620af376f196023edbbbce9e81
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35518433"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Education.SynchronizationProfiles["{id}"]
    .Pause()
    .Request()
    .PostAsync();

```