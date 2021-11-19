---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 97fc0e361d8e737ab345191dcfddc72a913d5741
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61083432"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetAddMembers( []UpdatableAsset {
    msgraphsdk.NewUpdatableAsset(),
    SetAdditionalData(map[string]interface{}{
        "@odata.type": "#microsoft.graph.windowsUpdates.updatableAsset",
        "id": "String (identifier)",
    }
}
requestBody.SetRemoveMembers( []UpdatableAsset {
    msgraphsdk.NewUpdatableAsset(),
    SetAdditionalData(map[string]interface{}{
        "@odata.type": "#microsoft.graph.windowsUpdates.updatableAsset",
        "id": "String (identifier)",
    }
}
requestBody.SetAddExclusions( []UpdatableAsset {
    msgraphsdk.NewUpdatableAsset(),
    SetAdditionalData(map[string]interface{}{
        "@odata.type": "#microsoft.graph.windowsUpdates.updatableAsset",
        "id": "String (identifier)",
    }
}
requestBody.SetRemoveExclusions( []UpdatableAsset {
    msgraphsdk.NewUpdatableAsset(),
    SetAdditionalData(map[string]interface{}{
        "@odata.type": "#microsoft.graph.windowsUpdates.updatableAsset",
        "id": "String (identifier)",
    }
}
options := &msgraphsdk.UpdateAudienceRequestBuilderPostOptions{
    Body: requestBody,
}
deploymentId := "deployment-id"
graphClient.Admin().Windows().Updates().DeploymentsById(&deploymentId).Audience().UpdateAudience().Post(options)


```