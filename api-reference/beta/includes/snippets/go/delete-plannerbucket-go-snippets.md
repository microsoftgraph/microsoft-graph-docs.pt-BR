---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 091928b27cab607e102aa92eb132178a4286f333
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411357"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

headers := map[string]string{
    "If-Match": "W/"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc=""
}
options := &msgraphsdk.PlannerBucketRequestBuilderDeleteOptions{
    H: headers,
}
plannerBucketId := "plannerBucket-id"
result, err := graphClient.Planner().BucketsById(&plannerBucketId).Delete(options)


```