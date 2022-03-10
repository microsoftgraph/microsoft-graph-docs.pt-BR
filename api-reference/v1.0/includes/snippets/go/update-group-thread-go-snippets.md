---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c7befd61f6c4d327a264c1609c9a1f49d88918a7
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2022
ms.locfileid: "63410978"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewConversationThread()
requestBody.SetAdditionalData(map[string]interface{}{
    "originalStartTimeZone": "originalStartTimeZone-value",
    "originalEndTimeZone": "originalEndTimeZone-value",
    "iCalUId": "iCalUId-value",
    "reminderMinutesBeforeStart": ,
    "isReminderOn": true,
}
options := &msgraphsdk.ConversationThreadRequestBuilderPatchOptions{
    Body: requestBody,
}
groupId := "group-id"
conversationThreadId := "conversationThread-id"
result, err := graphClient.GroupsById(&groupId).ThreadsById(&conversationThreadId).Patch(options)


```