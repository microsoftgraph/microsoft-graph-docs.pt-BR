---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4368e910d59475e441d43995c42ac71c74b89961
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62135550"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewMessage()
isRead := "true"
requestBody.SetIsRead(&isRead)
options := &msgraphsdk.MessageRequestBuilderPatchOptions{
    Body: requestBody,
}
messageId := "message-id"
graphClient.Me().MessagesById(&messageId).Patch(options)


```