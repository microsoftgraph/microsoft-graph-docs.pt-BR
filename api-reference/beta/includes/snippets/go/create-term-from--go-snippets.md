---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 46348eee0f7b769deee3ec814eb0add70b5a453f
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65323207"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewTerm()
requestBody.SetLabels( []LocalizedLabel {
    msgraphsdk.NewLocalizedLabel(),
    SetAdditionalData(map[string]interface{}{
        "languageTag": "en-US",
        "name": "Car",
        "isDefault": true,
    }
}
setId := "set-id"
result, err := graphClient.TermStore().SetsById(&setId).Children().Post(requestBody)


```