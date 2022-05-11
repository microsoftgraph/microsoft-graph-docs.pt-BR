---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b34cbc91fc33e2d5f8429f1156a1ca5281e4d8e8
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65325583"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

inferenceClassificationOverrideId := "inferenceClassificationOverride-id"
graphClient.Me().InferenceClassification().OverridesById(&inferenceClassificationOverrideId).Delete()


```