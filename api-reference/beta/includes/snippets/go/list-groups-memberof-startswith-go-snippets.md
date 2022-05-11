---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 88765b93f62add5127ae7acf78a74e5b9dc6baee
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65323452"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.DirectoryObjectRequestBuilderGetQueryParameters{
    Count: true,
    Orderby: "displayName",
    Filter: "startswith(displayName,%20'A')",
}
headers := map[string]string{
    "ConsistencyLevel": "eventual"
}
options := &msgraphsdk.DirectoryObjectRequestBuilderGetRequestConfiguration{
    QueryParameters: requestParameters,
    Headers: headers,
}
groupId := "group-id"
directoryObjectId := "directoryObject-id"
result, err := graphClient.GroupsById(&groupId).MemberOfById(&directoryObjectId).GetWithRequestConfigurationAndResponseHandler(options, nil)


```