---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e788c62ead117ea8326e8dff08c117f11465c107
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61009362"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.New()
updateCategory := "feature"
requestBody.SetUpdateCategory(&updateCategory)
memberEntityType := "#microsoft.graph.windowsUpdates.azureADDevice"
requestBody.SetMemberEntityType(&memberEntityType)
requestBody.SetIds( []String {
    "String",
    "String",
    "String",
}
options := &msgraphsdk.EnrollAssetsByIdRequestBuilderPostOptions{
    Body: requestBody,
}
graphClient.Admin().Windows().Updates().UpdatableAssets().EnrollAssetsById().Post(options)


```