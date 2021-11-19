---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 47449a3da5df2c2e5038edb796e44028ca852517
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61104135"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

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