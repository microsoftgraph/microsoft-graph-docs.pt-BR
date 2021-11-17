---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cb4f0e2f7f3b052fa23278e7875f2119a2a9c479
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "60990019"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

headers := map[string]string{
    "If-Match": "W/"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc=""
}
options := &msgraphsdk.PlannerTaskRequestBuilderDeleteOptions{
    H: headers,
}
plannerTaskId := "plannerTask-id"
graphClient.Planner().TasksById(&plannerTaskId).Delete(options)


```