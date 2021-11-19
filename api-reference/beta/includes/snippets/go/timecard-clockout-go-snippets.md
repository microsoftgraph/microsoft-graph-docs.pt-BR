---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1781dcbaa155b07e1aefc5a7203a7f48e8c8609d
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61091924"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
notes := msgraphsdk.NewItemBody()
requestBody.SetNotes(notes)
contentType := "text"
notes.SetContentType(&contentType)
content := "clock out smaple notes"
notes.SetContent(&content)
requestBody.SetAdditionalData(map[string]interface{}{
    "atAprovedLocation": true,
}
options := &msgraphsdk.ClockOutRequestBuilderPostOptions{
    Body: requestBody,
}
teamId := "team-id"
timeCardId := "timeCard-id"
result, err := graphClient.TeamsById(&teamId).Schedule().TimeCardsById(&timeCardId).ClockOut().Post(options)


```