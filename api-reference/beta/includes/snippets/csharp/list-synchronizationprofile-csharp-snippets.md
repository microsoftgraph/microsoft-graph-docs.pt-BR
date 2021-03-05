---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3df4574ba811ed9495dfb05cf17d8664a0c99ac0
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50470493"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var synchronizationProfiles = await graphClient.Education.SynchronizationProfiles
    .Request()
    .GetAsync();

```