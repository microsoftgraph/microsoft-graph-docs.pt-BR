---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bdbea13aa8e2f308e411ed095a66976816800ff5
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61102046"
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
options := &msgraphsdk.ContinuousAccessEvaluationPolicyRequestBuilderPatchOptions{
    Body: requestBody,
}
graphClient.Identity().ContinuousAccessEvaluationPolicy().Patch(options)


```