---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fb62a0f2dd3743fc83fe626215890341b0f69240
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65325063"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetSchedules( []String {
    "adelev@contoso.onmicrosoft.com",
    "meganb@contoso.onmicrosoft.com",
}
startTime := msgraphsdk.NewDateTimeTimeZone()
requestBody.SetStartTime(startTime)
dateTime := "2019-03-15T09:00:00"
startTime.SetDateTime(&dateTime)
timeZone := "Pacific Standard Time"
startTime.SetTimeZone(&timeZone)
endTime := msgraphsdk.NewDateTimeTimeZone()
requestBody.SetEndTime(endTime)
dateTime := "2019-03-15T18:00:00"
endTime.SetDateTime(&dateTime)
timeZone := "Pacific Standard Time"
endTime.SetTimeZone(&timeZone)
availabilityViewInterval := int32(60)
requestBody.SetAvailabilityViewInterval(&availabilityViewInterval)
headers := map[string]string{
    "Prefer": "outlook.timezone="Pacific Standard Time""
}
options := &msgraphsdk.GetScheduleRequestBuilderPostRequestConfiguration{
    Headers: headers,
}
result, err := graphClient.Me().Calendar().GetSchedule().PostWithRequestConfigurationAndResponseHandler(requestBody, options, nil)


```