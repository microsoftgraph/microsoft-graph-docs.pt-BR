---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 282ba5fdf342e78815a6bdbf3939a5bf9c458c67
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65322158"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.MembersRequestBuilderGetQueryParameters{
    Count: true,
    Filter: "startswith(displayName,%20'a')",
}
headers := map[string]string{
    "ConsistencyLevel": "eventual"
}
options := &msgraphsdk.MembersRequestBuilderGetRequestConfiguration{
    QueryParameters: requestParameters,
    Headers: headers,
}
groupId := "group-id"
result, err := graphClient.GroupsById(&groupId).Members().GetWithRequestConfigurationAndResponseHandler(options, nil)


```