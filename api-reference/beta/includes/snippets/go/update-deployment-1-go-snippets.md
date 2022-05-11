---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cccad8b4a77bb44c203aefcdce39be356bff6f0f
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65324370"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewDeployment()
state := msgraphsdk.NewDeploymentState()
requestBody.SetState(state)
requestedValue := "paused"
state.SetRequestedValue(&requestedValue)
state.SetAdditionalData(map[string]interface{}{
    "@odata.type": "microsoft.graph.windowsUpdates.deploymentState",
}
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.type": "#microsoft.graph.windowsUpdates.deployment",
}
deploymentId := "deployment-id"
graphClient.Admin().Windows().Updates().DeploymentsById(&deploymentId).Patch(requestBody)


```