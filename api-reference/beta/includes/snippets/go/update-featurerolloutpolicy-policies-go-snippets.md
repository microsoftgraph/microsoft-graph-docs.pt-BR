---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a8293027a666e8d9f527dfa0372c0e9407eff7b6
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65325589"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewFeatureRolloutPolicy()
displayName := "PasswordHashSync Rollout Policy"
requestBody.SetDisplayName(&displayName)
description := "PasswordHashSync Rollout Policy"
requestBody.SetDescription(&description)
isEnabled := true
requestBody.SetIsEnabled(&isEnabled)
isAppliedToOrganization := false
requestBody.SetIsAppliedToOrganization(&isAppliedToOrganization)
featureRolloutPolicyId := "featureRolloutPolicy-id"
graphClient.Policies().FeatureRolloutPoliciesById(&featureRolloutPolicyId).Patch(requestBody)


```