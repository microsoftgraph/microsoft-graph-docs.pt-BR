---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d9edc62ae79fc748c8f0b81422a4dc16bcf003f2
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65324375"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.UsersRequestBuilderGetQueryParameters{
    Filter: "endswith(mail,'a@contoso.com')",
    Orderby: "userPrincipalName",
    Count: true,
}
headers := map[string]string{
    "ConsistencyLevel": "eventual"
}
options := &msgraphsdk.UsersRequestBuilderGetRequestConfiguration{
    QueryParameters: requestParameters,
    Headers: headers,
}
result, err := graphClient.Users().GetWithRequestConfigurationAndResponseHandler(options, nil)


```