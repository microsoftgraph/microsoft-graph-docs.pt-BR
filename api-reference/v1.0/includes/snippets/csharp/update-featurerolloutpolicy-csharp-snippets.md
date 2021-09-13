---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f548c51450b8c29282ab14cab17bc77fac17b89ee197621f5518796bdac76f8c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158116"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var featureRolloutPolicy = new FeatureRolloutPolicy
{
    DisplayName = "PasswordHashSync Rollout Policy",
    Description = "PasswordHashSync Rollout Policy",
    IsEnabled = true,
    IsAppliedToOrganization = false
};

await graphClient.Policies.FeatureRolloutPolicies["{featureRolloutPolicy-id}"]
    .Request()
    .UpdateAsync(featureRolloutPolicy);

```