---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d4ffca3f008515df2aef6d07b0a9298dc0e8d0b1
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61004182"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestParameters := &msgraphsdk.UpdatableAssetsRequestBuilderGetQueryParameters{
    Filter: "isof('microsoft.graph.windowsUpdates.updatableAssetGroup')",
}
options := &msgraphsdk.UpdatableAssetsRequestBuilderGetOptions{
    Q: requestParameters,
}
result, err := graphClient.Admin().Windows().Updates().UpdatableAssets().Get(options)


```