---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 798b04e49bd013620af376f196023edbbbce9e81
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48604399"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Education.SynchronizationProfiles["{id}"]
    .Pause()
    .Request()
    .PostAsync();

```