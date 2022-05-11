---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 557132433ef5e9b1f2d2201976617a8101e353a0
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65324714"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.RegistrationRequestBuilderGetQueryParameters{
    Expand: "microsoft.graph.meetingRegistration/customQuestions",
}
options := &msgraphsdk.RegistrationRequestBuilderGetRequestConfiguration{
    QueryParameters: requestParameters,
}
onlineMeetingId := "onlineMeeting-id"
result, err := graphClient.Me().OnlineMeetingsById(&onlineMeetingId).Registration().GetWithRequestConfigurationAndResponseHandler(options, nil)


```