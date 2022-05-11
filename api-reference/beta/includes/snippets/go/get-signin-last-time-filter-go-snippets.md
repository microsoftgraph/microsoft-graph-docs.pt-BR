---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 972a432e03e4f6a7d39adfb2c5067412abd075b2
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65324378"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.UsersRequestBuilderGetQueryParameters{
    Filter: "startswith(displayName,'Eric')",
    Select: "displayName,signInActivity",
}
options := &msgraphsdk.UsersRequestBuilderGetRequestConfiguration{
    QueryParameters: requestParameters,
}
result, err := graphClient.Users().GetWithRequestConfigurationAndResponseHandler(options, nil)


```