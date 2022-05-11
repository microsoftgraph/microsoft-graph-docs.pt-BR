---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a315f7cbfbd7ed0979147ec6976233a080ae19de
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65324482"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
comment := "comment-value"
requestBody.SetComment(&comment)
requestBody.SetToRecipients( []Recipient {
    msgraphsdk.NewRecipient(),
    SetAdditionalData(map[string]interface{}{
    }
}
messageId := "message-id"
graphClient.Me().MessagesById(&messageId).Forward(message-id).Post(requestBody)


```