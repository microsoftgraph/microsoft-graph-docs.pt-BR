---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3b53f1f53fca7ca45424e85c4ac2745db6831c45
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65323761"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.FeatureRolloutPolicyRequestBuilderGetQueryParameters{
    Expand: "appliesTo",
}
options := &msgraphsdk.FeatureRolloutPolicyRequestBuilderGetRequestConfiguration{
    QueryParameters: requestParameters,
}
featureRolloutPolicyId := "featureRolloutPolicy-id"
result, err := graphClient.Policies().FeatureRolloutPoliciesById(&featureRolloutPolicyId).GetWithRequestConfigurationAndResponseHandler(options, nil)


```