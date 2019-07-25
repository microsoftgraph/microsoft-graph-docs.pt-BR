---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4a02b66cb311bbc274e643b5cee2c1e43b3ba883
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35712461"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Education.SynchronizationProfiles["{id}"]
    .Reset()
    .Request()
    .PostAsync();

```