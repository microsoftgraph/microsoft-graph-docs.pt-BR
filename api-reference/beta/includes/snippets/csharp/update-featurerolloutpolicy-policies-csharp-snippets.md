---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b935558b58b7343d9e4c540bbf21410cf81da676
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/02/2021
ms.locfileid: "51508587"
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