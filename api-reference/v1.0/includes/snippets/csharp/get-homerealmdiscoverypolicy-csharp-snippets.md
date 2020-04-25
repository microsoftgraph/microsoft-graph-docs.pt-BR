---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 478474250ba5dcb1a8dc1c89028266220f3fb817
ms.sourcegitcommit: 5575e6607817ba23ceb0b01e2f5fc81e58bdcd1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43805580"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var homeRealmDiscoveryPolicy = await graphClient.Policies.HomeRealmDiscoveryPolicies["{id}"]
    .Request()
    .GetAsync();

```