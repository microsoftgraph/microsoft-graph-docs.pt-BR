---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: aa671ca0c228d3504ffd861ef62b4c98a50511ce
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61012623"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestParameters := &msgraphsdk.EventsRequestBuilderGetQueryParameters{
    Filter: "startsWith(subject,'All')",
}
options := &msgraphsdk.EventsRequestBuilderGetOptions{
    Q: requestParameters,
}
result, err := graphClient.Me().Calendar().Events().Get(options)


```