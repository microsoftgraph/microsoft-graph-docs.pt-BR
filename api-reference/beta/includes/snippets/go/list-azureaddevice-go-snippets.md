---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 10d66aff48e0cc2b3d85e1833e22dd3901f08d06
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65324368"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.UpdatableAssetsRequestBuilderGetQueryParameters{
    Filter: "isof('microsoft.graph.windowsUpdates.azureADDevice')",
}
options := &msgraphsdk.UpdatableAssetsRequestBuilderGetRequestConfiguration{
    QueryParameters: requestParameters,
}
result, err := graphClient.Admin().Windows().Updates().UpdatableAssets().GetWithRequestConfigurationAndResponseHandler(options, nil)


```