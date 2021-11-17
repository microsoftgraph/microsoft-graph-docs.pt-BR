---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e0c7e6604162fd1615462ada0e25e703adc62e6d
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "60988535"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestParameters := &msgraphsdk.UsedRequestBuilderGetQueryParameters{
    Orderby: "LastUsed/LastAccessedDateTime%20desc",
}
options := &msgraphsdk.UsedRequestBuilderGetOptions{
    Q: requestParameters,
}
result, err := graphClient.Me().Insights().Used().Get(options)


```