---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 989ee095c12f93435d2463b276f00971fa8a5477
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61096698"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.PendingAccessReviewInstancesRequestBuilderGetQueryParameters{
    Expand: "definition",
    Top: 100,
    Skip: 0,
}
options := &msgraphsdk.PendingAccessReviewInstancesRequestBuilderGetOptions{
    Q: requestParameters,
}
result, err := graphClient.Me().PendingAccessReviewInstances().Get(options)


```