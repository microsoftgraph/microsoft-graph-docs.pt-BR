---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1b2d5415b5251a5d5d60fc5904b6eeeecaee3e02
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61023383"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewMessage()
receivedDateTime, err := time.Parse(time.RFC3339, "datetime-value")
requestBody.SetReceivedDateTime(&receivedDateTime)
sentDateTime, err := time.Parse(time.RFC3339, "datetime-value")
requestBody.SetSentDateTime(&sentDateTime)
hasAttachments := true
requestBody.SetHasAttachments(&hasAttachments)
subject := "subject-value"
requestBody.SetSubject(&subject)
body := msgraphsdk.NewItemBody()
requestBody.SetBody(body)
contentType := ""
body.SetContentType(&contentType)
content := "content-value"
body.SetContent(&content)
bodyPreview := "bodyPreview-value"
requestBody.SetBodyPreview(&bodyPreview)
options := &msgraphsdk.MessagesRequestBuilderPostOptions{
    Body: requestBody,
}
mailFolderId := "mailFolder-id"
result, err := graphClient.Me().MailFoldersById(&mailFolderId).Messages().Post(options)


```