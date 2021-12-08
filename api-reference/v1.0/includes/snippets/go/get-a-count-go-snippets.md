---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ac71f981de7b05359f891d1fa6b0a1b1b01ed833
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2021
ms.locfileid: "61348750"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.GroupsRequestBuilderGetQueryParameters{
    Filter: "startswith(displayName,%20'a')",
    Count: true,
    Top: 1,
    Orderby: "displayName",
}
headers := map[string]string{
    "ConsistencyLevel": "eventual"
}
options := &msgraphsdk.GroupsRequestBuilderGetOptions{
    Q: requestParameters,
    H: headers,
}
result, err := graphClient.Groups().Get(options)


```