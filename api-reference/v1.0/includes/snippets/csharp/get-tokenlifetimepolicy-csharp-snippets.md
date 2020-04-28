---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 904d8605493f40fd05b35210d31d983d2a69e072
ms.sourcegitcommit: 5575e6607817ba23ceb0b01e2f5fc81e58bdcd1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43719225"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tokenLifetimePolicy = await graphClient.Policies.TokenLifetimePolicies["{id}"]
    .Request()
    .GetAsync();

```