---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 02b49c184296a00a08b6c212ab2f3246f7d9c79a
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65322609"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.AccessReviewInstanceDecisionItemRequestBuilderGetQueryParameters{
    Expand: "instance($expand=definition)",
}
options := &msgraphsdk.AccessReviewInstanceDecisionItemRequestBuilderGetRequestConfiguration{
    QueryParameters: requestParameters,
}
accessReviewInstanceDecisionItemId := "accessReviewInstanceDecisionItem-id"
result, err := graphClient.IdentityGovernance().AccessReviews().DecisionsById(&accessReviewInstanceDecisionItemId).GetWithRequestConfigurationAndResponseHandler(options, nil)


```