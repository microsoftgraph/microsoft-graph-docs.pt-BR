---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b708f8d6607bfe87f21fe2fa3bf5bdcf8a0224c9
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65324121"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetParticipants( []String {
    "",
}
clientContext := "clientContext-value"
requestBody.SetClientContext(&clientContext)
callId := "call-id"
result, err := graphClient.Communications().CallsById(&callId).Participants().MuteAll(call-id).Post(requestBody)


```