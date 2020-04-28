---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c30c4ecc76b3c233d214b1ab3957bb8950d6c3aa
ms.sourcegitcommit: 5575e6607817ba23ceb0b01e2f5fc81e58bdcd1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43805425"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tokenIssuancePolicy = await graphClient.Policies.TokenIssuancePolicies["{id}"]
    .Request()
    .GetAsync();

```