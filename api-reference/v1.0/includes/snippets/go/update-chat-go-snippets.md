---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: eaf54e3630d19a3e2d689199103966d7dabeeefd
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61099077"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewChat()
topic := "Group chat title update"
requestBody.SetTopic(&topic)
options := &msgraphsdk.ChatRequestBuilderPatchOptions{
    Body: requestBody,
}
chatId := "chat-id"
graphClient.ChatsById(&chatId).Patch(options)


```