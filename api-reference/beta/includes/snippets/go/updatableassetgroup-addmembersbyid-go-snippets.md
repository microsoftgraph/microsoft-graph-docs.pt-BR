---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: eecb7fd89b336d3eec39216cee6a73e03693701d
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65323844"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetIds( []String {
    "String",
    "String",
    "String",
}
memberEntityType := "#microsoft.graph.windowsUpdates.azureADDevice"
requestBody.SetMemberEntityType(&memberEntityType)
updatableAssetId := "updatableAsset-id"
graphClient.Admin().Windows().Updates().UpdatableAssetsById(&updatableAssetId).AddMembersById(updatableAsset-id).Post(requestBody)


```