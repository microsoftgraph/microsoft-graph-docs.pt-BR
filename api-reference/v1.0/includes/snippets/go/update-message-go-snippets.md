---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7660ea74a291f3cf1e2f7e2a467279b5961f428a
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65325393"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewMessage()
subject := "subject-value"
requestBody.SetSubject(&subject)
body := msgraphsdk.NewItemBody()
requestBody.SetBody(body)
contentType := ""
body.SetContentType(&contentType)
content := "content-value"
body.SetContent(&content)
inferenceClassification := "other"
requestBody.SetInferenceClassification(&inferenceClassification)
messageId := "message-id"
graphClient.Me().MessagesById(&messageId).Patch(requestBody)


```