---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ab6db90b8c056823023f6753a0cf2b296dc12725
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "60977586"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewTerm()
requestBody.SetLabels( []LocalizedLabel {
    msgraphsdk.NewLocalizedLabel(),
    SetAdditionalData(map[string]interface{}{
        "languageTag": "en-US",
        "name": "Car",
        "isDefault": true,
    }
}
options := &msgraphsdk.ChildrenRequestBuilderPostOptions{
    Body: requestBody,
}
setId := "set-id"
result, err := graphClient.TermStore().SetsById(&setId).Children().Post(options)


```