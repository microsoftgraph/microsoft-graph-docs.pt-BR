---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 33351750aec15f0ed2e5f4851022adbd1e62cd59
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411487"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewCommentRequestBody()
comment := "Cancelling for this week due to all hands"
requestBody.SetComment(&comment)
options := &msgraphsdk.CancelRequestBuilderPostOptions{
    Body: requestBody,
}
eventId := "event-id"
graphClient.Me().EventsById(&eventId).Cancel(event-id).Post(options)


```