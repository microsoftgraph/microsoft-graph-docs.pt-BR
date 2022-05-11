---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 347cbec2d2fd3712bd227b3352b6823cf1d2e8bd
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65323413"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.DefinitionsRequestBuilderGetQueryParameters{
    Filter: "contains(scope/microsoft.graph.accessReviewQueryScope/query,%20'./members')",
}
options := &msgraphsdk.DefinitionsRequestBuilderGetRequestConfiguration{
    QueryParameters: requestParameters,
}
result, err := graphClient.IdentityGovernance().AccessReviews().Definitions().GetWithRequestConfigurationAndResponseHandler(options, nil)


```