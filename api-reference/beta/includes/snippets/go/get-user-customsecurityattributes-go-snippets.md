---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 04ba7e230e524ca56d510129f41e4b2fdae11b05
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65325216"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.UserRequestBuilderGetQueryParameters{
    Select: "customSecurityAttributes",
}
options := &msgraphsdk.UserRequestBuilderGetRequestConfiguration{
    QueryParameters: requestParameters,
}
userId := "user-id"
result, err := graphClient.UsersById(&userId).GetWithRequestConfigurationAndResponseHandler(options, nil)


```