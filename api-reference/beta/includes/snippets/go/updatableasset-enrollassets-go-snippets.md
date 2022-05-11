---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e614be65e69d5603f3d73f72ca527e3c06e72271
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65324996"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
updateCategory := "String"
requestBody.SetUpdateCategory(&updateCategory)
requestBody.SetAssets( []UpdatableAsset {
    msgraphsdk.NewUpdatableAsset(),
    SetAdditionalData(map[string]interface{}{
        "@odata.type": "#microsoft.graph.windowsUpdates.azureADDevice",
        "id": "String (identifier)",
    }
}
graphClient.Admin().Windows().Updates().UpdatableAssets().EnrollAssets().Post(requestBody)


```