---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 037dcd5ae864506479564d6aadb01dc115eee31c
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62123541"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.type": "#microsoft.graph.externalMeetingRegistration",
    "allowedRegistrant": "everyone",
}
options := &msgraphsdk.RegistrationRequestBuilderPostOptions{
    Body: requestBody,
}
onlineMeetingId := "onlineMeeting-id"
graphClient.Me().OnlineMeetingsById(&onlineMeetingId).Registration().Post(options)


```