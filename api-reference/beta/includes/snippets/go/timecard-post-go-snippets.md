---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 20cafe3dbf6ddc8a17306e841b2b52d6afc3b67f
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65323084"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewTimeCard()
clockInEvent := msgraphsdk.NewTimeCardEvent()
requestBody.SetClockInEvent(clockInEvent)
dateTime, err := time.Parse(time.RFC3339, "2019-03-18T00:00:00.000Z")
clockInEvent.SetDateTime(&dateTime)
atApprovedLocation := true
clockInEvent.SetAtApprovedLocation(&atApprovedLocation)
notes := msgraphsdk.NewItemBody()
clockInEvent.SetNotes(notes)
content := "Started late due to traffic in CA 237"
notes.SetContent(&content)
contentType := "text"
notes.SetContentType(&contentType)
notes := msgraphsdk.NewItemBody()
requestBody.SetNotes(notes)
content := "8 To 5 Inventory management"
notes.SetContent(&content)
contentType := "text"
notes.SetContentType(&contentType)
requestBody.SetBreaks( []TimeCardBreak {
    msgraphsdk.NewTimeCardBreak(),
    SetAdditionalData(map[string]interface{}{
        "breakId": "string",
    }
}
requestBody.SetAdditionalData(map[string]interface{}{
    "onBehalfOfUserId": "a3601044-a1b5-438e-b742-f78d01d68a67",
}
teamId := "team-id"
result, err := graphClient.TeamsById(&teamId).Schedule().TimeCards().Post(requestBody)


```