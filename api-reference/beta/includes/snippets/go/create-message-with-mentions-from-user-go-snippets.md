---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cf4664dcd2a2154151cce1945226dde37fbca0fe
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65322789"
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
result, err := graphClient.Me().Messages().Post(requestBody)


```