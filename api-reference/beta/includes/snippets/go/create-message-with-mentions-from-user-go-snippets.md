---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bb7a3a121ce489546541bd120ec484a52600cab0
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "60985091"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

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