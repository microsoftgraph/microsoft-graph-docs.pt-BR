---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a3370f8a1e39ef8e723ee13ff545d6f2ceb5a886
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61008439"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestParameters := &msgraphsdk.MeRequestBuilderGetQueryParameters{
    Expand: "manager($levels=max;$select=id,displayName)",
    Select: "id,displayName",
    Count: true,
}
headers := map[string]string{
    "ConsistencyLevel": "eventual"
}
options := &msgraphsdk.MeRequestBuilderGetOptions{
    Q: requestParameters,
    H: headers,
}
result, err := graphClient.Me().Get(options)


```