---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 15592aebf35cc4d8c490a3eda885b9c644fcec26
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "60985491"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewPlannerRoster()
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.type": "#microsoft.graph.plannerRoster",
}
options := &msgraphsdk.RostersRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Planner().Rosters().Post(options)


```