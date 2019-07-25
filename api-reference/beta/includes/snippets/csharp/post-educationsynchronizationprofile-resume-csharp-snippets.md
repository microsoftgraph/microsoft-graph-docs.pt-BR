---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1193daaf5dc8fbabb1000952d3b2ba15a0ffed6c
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35714400"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Education.SynchronizationProfiles["{id}"]
    .Resume()
    .Request()
    .PostAsync();

```