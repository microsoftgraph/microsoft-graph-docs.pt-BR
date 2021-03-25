---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f6db16241a5aa507ae850890047d7d9521a28154
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51201573"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

FeatureRolloutPolicy featureRolloutPolicy = new FeatureRolloutPolicy();
featureRolloutPolicy.displayName = "PassthroughAuthentication rollout policy";
featureRolloutPolicy.description = "PassthroughAuthentication rollout policy";
featureRolloutPolicy.feature = StagedFeatureName.PASSTHROUGH_AUTHENTICATION;
featureRolloutPolicy.isEnabled = true;
featureRolloutPolicy.isAppliedToOrganization = false;

graphClient.policies().featureRolloutPolicies()
    .buildRequest()
    .post(featureRolloutPolicy);

```