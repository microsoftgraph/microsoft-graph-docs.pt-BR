---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2a6e9907bd9c810a1431a1481c2b71a9973e1528
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65324833"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
message := msgraphsdk.NewMessage()
requestBody.SetMessage(message)
isDeliveryReceiptRequested := true
message.SetIsDeliveryReceiptRequested(&isDeliveryReceiptRequested)
message.SetToRecipients( []Recipient {
    msgraphsdk.NewRecipient(),
    SetAdditionalData(map[string]interface{}{
    }
}
comment := "Dana, just want to make sure you get this; you'll need this if the project gets approved."
requestBody.SetComment(&comment)
messageId := "message-id"
result, err := graphClient.Me().MessagesById(&messageId).CreateForward(message-id).Post(requestBody)


```