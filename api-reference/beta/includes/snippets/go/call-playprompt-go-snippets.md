---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 207d29c986cf5ac10ce01da18834485883e1c2ea
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65323366"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
clientContext := "d45324c1-fcb5-430a-902c-f20af696537c"
requestBody.SetClientContext(&clientContext)
requestBody.SetPrompts( []Prompt {
    msgraphsdk.NewPrompt(),
    SetAdditionalData(map[string]interface{}{
        "@odata.type": "#microsoft.graph.mediaPrompt",
    }
}
loop := false
requestBody.SetLoop(&loop)
callId := "call-id"
result, err := graphClient.Communications().CallsById(&callId).PlayPrompt(call-id).Post(requestBody)


```