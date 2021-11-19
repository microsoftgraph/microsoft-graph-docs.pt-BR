---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a8aca84c247a461ba1bac8b2291ab5ad82ae9c0b
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61102004"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetAssets( []UpdatableAsset {
    msgraphsdk.NewUpdatableAsset(),
    SetAdditionalData(map[string]interface{}{
        "@odata.type": "#microsoft.graph.windowsUpdates.azureADDevice",
        "id": "String (identifier)",
    }
}
options := &msgraphsdk.RemoveMembersRequestBuilderPostOptions{
    Body: requestBody,
}
updatableAssetId := "updatableAsset-id"
graphClient.Admin().Windows().Updates().UpdatableAssetsById(&updatableAssetId).RemoveMembers().Post(options)


```