---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1b588816f20c00691d98df2afdb93c679675c90b
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65323031"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewContinuousAccessEvaluationPolicy()
migrate := true
requestBody.SetMigrate(&migrate)
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.type": "#microsoft.graph.continuousAccessEvaluationPolicy",
}
graphClient.Identity().ContinuousAccessEvaluationPolicy().Patch(requestBody)


```