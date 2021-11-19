---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5f505dbbc4ee0ed61da68c12f2bbbe8c17a1d80e
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61093481"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
newReminderTime := msgraphsdk.NewDateTimeTimeZone()
requestBody.SetNewReminderTime(newReminderTime)
dateTime := "dateTime-value"
newReminderTime.SetDateTime(&dateTime)
timeZone := "timeZone-value"
newReminderTime.SetTimeZone(&timeZone)
options := &msgraphsdk.SnoozeReminderRequestBuilderPostOptions{
    Body: requestBody,
}
eventId := "event-id"
graphClient.Me().EventsById(&eventId).SnoozeReminder().Post(options)


```