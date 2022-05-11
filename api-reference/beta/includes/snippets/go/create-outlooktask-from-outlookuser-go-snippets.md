---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f477ae761122773edad7a313b46cdfd10dfb2658
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65323322"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewOutlookTask()
subject := "Shop for children's weekend"
requestBody.SetSubject(&subject)
startDateTime := msgraphsdk.NewDateTimeTimeZone()
requestBody.SetStartDateTime(startDateTime)
dateTime := "2016-05-03T09:00:00"
startDateTime.SetDateTime(&dateTime)
timeZone := "Eastern Standard Time"
startDateTime.SetTimeZone(&timeZone)
dueDateTime := msgraphsdk.NewDateTimeTimeZone()
requestBody.SetDueDateTime(dueDateTime)
dateTime := "2016-05-05T16:00:00"
dueDateTime.SetDateTime(&dateTime)
timeZone := "Eastern Standard Time"
dueDateTime.SetTimeZone(&timeZone)
headers := map[string]string{
    "Prefer": "outlook.timezone="Pacific Standard Time""
}
options := &msgraphsdk.TasksRequestBuilderPostRequestConfiguration{
    Headers: headers,
}
result, err := graphClient.Me().Outlook().Tasks().PostWithRequestConfigurationAndResponseHandler(requestBody, options, nil)


```