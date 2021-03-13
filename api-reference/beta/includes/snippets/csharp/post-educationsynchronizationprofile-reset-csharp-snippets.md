---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 19cb9ac72b270cafd389adc8678127d45f6bba80
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50791863"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Education.SynchronizationProfiles["{educationSynchronizationProfile-id}"]
    .Reset()
    .Request()
    .PostAsync();

```