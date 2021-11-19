---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ac21dfa12dd747491ea513cd9ee07ff4922a6e80
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61094417"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewMessage()
subject := "Party planning"
requestBody.SetSubject(&subject)
requestBody.SetToRecipients( []Recipient {
    msgraphsdk.NewRecipient(),
    SetAdditionalData(map[string]interface{}{
    }
}
requestBody.SetMentions( []Mention {
    msgraphsdk.NewMention(),
    SetAdditionalData(map[string]interface{}{
    }
}
options := &msgraphsdk.MessagesRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Me().Messages().Post(options)


```