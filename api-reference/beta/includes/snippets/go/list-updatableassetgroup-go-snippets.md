---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ae503042a1ed87cf3a9e274410c3e0072b32e85e
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61084035"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.UpdatableAssetsRequestBuilderGetQueryParameters{
    Filter: "isof('microsoft.graph.windowsUpdates.updatableAssetGroup')",
}
options := &msgraphsdk.UpdatableAssetsRequestBuilderGetOptions{
    Q: requestParameters,
}
result, err := graphClient.Admin().Windows().Updates().UpdatableAssets().Get(options)


```