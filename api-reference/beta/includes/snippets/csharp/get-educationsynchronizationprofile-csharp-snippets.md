---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 592017c0ff09d8f802ed0037d470e91342825371
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50470383"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationSynchronizationProfile = await graphClient.Education.SynchronizationProfiles["{id}"]
    .Request()
    .GetAsync();

```