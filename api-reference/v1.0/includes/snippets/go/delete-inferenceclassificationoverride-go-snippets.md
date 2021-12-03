---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 757a7a67521fc95dd2b139f33d6bfc2143c3babb
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61286478"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

inferenceClassificationOverrideId := "inferenceClassificationOverride-id"
graphClient.Me().InferenceClassification().OverridesById(&inferenceClassificationOverrideId).Delete(nil)


```