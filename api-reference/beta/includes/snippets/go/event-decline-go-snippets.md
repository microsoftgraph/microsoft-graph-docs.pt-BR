---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3ddb2087fbf33d4c717ddc5ec7d3ff92385ab087
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65324589"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
comment := "I won't be able to make this week. How about next week?"
requestBody.SetComment(&comment)
sendResponse := true
requestBody.SetSendResponse(&sendResponse)
proposedNewTime := msgraphsdk.NewTimeSlot()
requestBody.SetProposedNewTime(proposedNewTime)
start := msgraphsdk.NewDateTimeTimeZone()
proposedNewTime.SetStart(start)
dateTime := "2019-12-02T18:00:00"
start.SetDateTime(&dateTime)
timeZone := "Pacific Standard Time"
start.SetTimeZone(&timeZone)
end := msgraphsdk.NewDateTimeTimeZone()
proposedNewTime.SetEnd(end)
dateTime := "2019-12-02T19:00:00"
end.SetDateTime(&dateTime)
timeZone := "Pacific Standard Time"
end.SetTimeZone(&timeZone)
eventId := "event-id"
graphClient.Me().EventsById(&eventId).Decline(event-id).Post(requestBody)


```