---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bf8e82b2c31bd2ecf6b83fd6fa37e8366858c092
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65324825"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewPlannerRoster()
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.type": "#microsoft.graph.plannerRoster",
}
result, err := graphClient.Planner().Rosters().Post(requestBody)


```