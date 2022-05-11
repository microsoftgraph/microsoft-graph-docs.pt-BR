---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6f4cf0865c5b1b71fcf2372d1517aabfe5a5403e
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65324035"
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
graphClient.Admin().Windows().Updates().UpdatableAssetsById(&updatableAssetId).RemoveMembers(updatableAsset-id).Post(requestBody)


```