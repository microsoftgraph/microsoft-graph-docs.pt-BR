---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f12df7f5988324da728dd71fd30f4bbad9ded9c9
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65324551"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

updatableAssetId := "updatableAsset-id"
result, err := graphClient.Admin().Windows().Updates().UpdatableAssetsById(&updatableAssetId).Get()


```