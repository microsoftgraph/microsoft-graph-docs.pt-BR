---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4d5771d2eecef4a602371a4104af67754e8aff4a
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65322606"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.PendingAccessReviewInstancesRequestBuilderGetQueryParameters{
    Expand: "definition",
    Top: 100,
    Skip: 0,
}
options := &msgraphsdk.PendingAccessReviewInstancesRequestBuilderGetRequestConfiguration{
    QueryParameters: requestParameters,
}
result, err := graphClient.Me().PendingAccessReviewInstances().GetWithRequestConfigurationAndResponseHandler(options, nil)


```