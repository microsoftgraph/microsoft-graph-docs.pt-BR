---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e4861308a3a430d797ccb2541188ea72fe9b1e3a
ms.sourcegitcommit: 8e18d7fe3c869b2fd48872365116175d3bdce1b7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/12/2020
ms.locfileid: "46643741"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var credentials = new List<SynchronizationSecretKeyStringValuePair>()
{
    new SynchronizationSecretKeyStringValuePair
    {
    }
};

await graphClient.Applications["{applicationsId}"].Synchronization
    .AcquireAccessToken(credentials)
    .Request()
    .PostAsync();

```