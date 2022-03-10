---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3cbc6bd75116ce92c6ed4105c6971bf91805bc9c
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411516"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

updatableAssetId := "updatableAsset-id"
result, err := graphClient.Admin().Windows().Updates().UpdatableAssetsById(&updatableAssetId).Delete(nil)


```