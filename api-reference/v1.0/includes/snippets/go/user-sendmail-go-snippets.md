---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 956d2ebd3bcd61b0c165f5596df1994b9d9c4df1
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65323924"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
message := msgraphsdk.NewMessage()
requestBody.SetMessage(message)
subject := "Meet for lunch?"
message.SetSubject(&subject)
body := msgraphsdk.NewItemBody()
message.SetBody(body)
contentType := "Text"
body.SetContentType(&contentType)
content := "The new cafeteria is open."
body.SetContent(&content)
message.SetToRecipients( []Recipient {
    msgraphsdk.NewRecipient(),
    SetAdditionalData(map[string]interface{}{
    }
}
message.SetCcRecipients( []Recipient {
    msgraphsdk.NewRecipient(),
    SetAdditionalData(map[string]interface{}{
    }
}
saveToSentItems := "false"
requestBody.SetSaveToSentItems(&saveToSentItems)
graphClient.Me().SendMail().Post(requestBody)


```