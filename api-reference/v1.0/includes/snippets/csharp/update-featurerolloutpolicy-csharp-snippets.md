---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b935558b58b7343d9e4c540bbf21410cf81da676
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51201249"
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