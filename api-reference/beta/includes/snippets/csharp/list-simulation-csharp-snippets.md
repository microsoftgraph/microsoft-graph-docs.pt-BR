---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 357a64fc44d23fb734c865b28c37f053fb8c332a
ms.sourcegitcommit: 36bae3615df41876493b25da478e589d1974f97b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/29/2021
ms.locfileid: "59995966"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var simulations = await graphClient.Security.AttackSimulation.Simulations
    .Request()
    .GetAsync();

```