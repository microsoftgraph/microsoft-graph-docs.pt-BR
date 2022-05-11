---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 82c700f4d5b41a90e20c280ca09902acdbb9d604
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65323220"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

featureRolloutPolicyId := "featureRolloutPolicy-id"
graphClient.Policies().FeatureRolloutPoliciesById(&featureRolloutPolicyId).Delete()


```