---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1193daaf5dc8fbabb1000952d3b2ba15a0ffed6c
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48614906"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Education.SynchronizationProfiles["{id}"]
    .Resume()
    .Request()
    .PostAsync();

```