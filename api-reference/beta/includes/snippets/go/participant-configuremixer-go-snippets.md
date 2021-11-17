---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a41dd59d8f9de34f1a273512ed045a82ce0081f1
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61018279"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.New()
requestBody.SetAdditionalData(map[string]interface{}{
    "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c",
    "participantMixerLevels":  []Object {
    }
}
options := &msgraphsdk.ParticipantRequestBuilderPostOptions{
    Body: requestBody,
}
callId := "call-id"
participantId := "participant-id"
graphClient.Communications().CallsById(&callId).ParticipantsById(&participantId).Post(options)


```