---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e6adcea57a77409213f7899e6181e1ef5043ce12
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65325461"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.ServicePrincipalsRequestBuilderGetQueryParameters{
    Filter: "startswith(displayName,%20'a')",
    Count: true,
    Top: 1,
    Orderby: "displayName",
}
headers := map[string]string{
    "ConsistencyLevel": "eventual"
}
options := &msgraphsdk.ServicePrincipalsRequestBuilderGetRequestConfiguration{
    QueryParameters: requestParameters,
    Headers: headers,
}
result, err := graphClient.ServicePrincipals().GetWithRequestConfigurationAndResponseHandler(options, nil)


```