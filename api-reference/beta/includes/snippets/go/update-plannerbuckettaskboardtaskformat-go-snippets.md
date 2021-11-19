---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 94edb808c715b2406f5e0ee314d94516cd0c2297
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61100702"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewPlannerBucketTaskBoardTaskFormat()
orderHint := "A6673H Ejkl!"
requestBody.SetOrderHint(&orderHint)
headers := map[string]string{
    "Prefer": "return=representation"
    "If-Match": "W/"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc=""
}
options := &msgraphsdk.BucketTaskBoardFormatRequestBuilderPatchOptions{
    Body: requestBody,
    H: headers,
}
plannerTaskId := "plannerTask-id"
graphClient.Planner().TasksById(&plannerTaskId).BucketTaskBoardFormat().Patch(options)


```