---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5c24062089b772fb737848de0df18357cf47973d
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61000703"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewChat()
topic := "Group chat title update"
requestBody.SetTopic(&topic)
options := &msgraphsdk.ChatRequestBuilderPatchOptions{
    Body: requestBody,
}
chatId := "chat-id"
graphClient.ChatsById(&chatId).Patch(options)


```