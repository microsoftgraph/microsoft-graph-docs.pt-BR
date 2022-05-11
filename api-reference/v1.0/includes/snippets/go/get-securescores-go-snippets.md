---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e7dcc900af57921290ea5d1a06a90514d00b3416
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65324199"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.SecureScoresRequestBuilderGetQueryParameters{
    Top: 1,
}
options := &msgraphsdk.SecureScoresRequestBuilderGetRequestConfiguration{
    QueryParameters: requestParameters,
}
result, err := graphClient.Security().SecureScores().GetWithRequestConfigurationAndResponseHandler(options, nil)


```