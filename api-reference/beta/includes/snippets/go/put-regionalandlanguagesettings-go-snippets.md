---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 07abe8652052f5090761c5abe9797f476b9259bc
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65324319"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetAdditionalData(map[string]interface{}{
    "authoringLanguages":  []Object {
    }
}
graphClient.Me().Settings().RegionalAndLanguageSettings().Put(requestBody)


```