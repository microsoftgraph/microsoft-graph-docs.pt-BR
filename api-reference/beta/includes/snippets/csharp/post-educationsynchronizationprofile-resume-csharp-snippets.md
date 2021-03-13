---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 347d6e81f6d584787be971f6b7be6492096228f9
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50786801"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Education.SynchronizationProfiles["{educationSynchronizationProfile-id}"]
    .Resume()
    .Request()
    .PostAsync();

```