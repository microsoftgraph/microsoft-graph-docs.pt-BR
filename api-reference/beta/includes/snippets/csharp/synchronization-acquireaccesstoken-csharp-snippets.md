---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 34828d3e3f34e0796aafd8091574554d91ac15faee4ab72c4fa436a3b9e1c96c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57214495"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var credentials = new List<SynchronizationSecretKeyStringValuePair>()
{
    new SynchronizationSecretKeyStringValuePair
    {
    }
};

await graphClient.Applications["{application-id}"].Synchronization
    .AcquireAccessToken(credentials)
    .Request()
    .PostAsync();

```