---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 926a1745b2737efa3445441d81bf846912081f2c
ms.sourcegitcommit: c4d6ccd343a6b298a2aa844f1bad66c736487251
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2020
ms.locfileid: "42593475"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var homeRealmDiscoveryPolicies = await graphClient.Policies.HomeRealmDiscoveryPolicies
    .Request()
    .GetAsync();

```