---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 061c092c44e7e2fed9cd974fb2c9bf4b4907688c
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65325674"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewAssetsRequestBody()
requestBody.SetAssets( []UpdatableAsset {
    msgraphsdk.NewUpdatableAsset(),
    SetAdditionalData(map[string]interface{}{
        "@odata.type": "#microsoft.graph.windowsUpdates.azureADDevice",
        "id": "String (identifier)",
    }
}
updatableAssetId := "updatableAsset-id"
graphClient.Admin().Windows().Updates().UpdatableAssetsById(&updatableAssetId).AddMembers(updatableAsset-id).Post(requestBody)


```