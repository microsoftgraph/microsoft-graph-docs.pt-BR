---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c0fd3d6c48a11c78f4bcdffc7ed44c2c4b7c9a36
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61088296"
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
message.SetAttachments( []Attachment {
    msgraphsdk.NewAttachment(),
    SetAdditionalData(map[string]interface{}{
        "@odata.type": "#microsoft.graph.fileAttachment",
        "name": "attachment.txt",
        "contentType": "text/plain",
        "contentBytes": "SGVsbG8gV29ybGQh",
    }
}
options := &msgraphsdk.SendMailRequestBuilderPostOptions{
    Body: requestBody,
}
graphClient.Me().SendMail().Post(options)


```