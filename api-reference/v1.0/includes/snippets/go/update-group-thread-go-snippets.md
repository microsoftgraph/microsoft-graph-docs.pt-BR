---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 012ce7a394c2aa1e02ed02e69ffa8639b328b527
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65323173"
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
groupId := "group-id"
conversationThreadId := "conversationThread-id"
graphClient.GroupsById(&groupId).ThreadsById(&conversationThreadId).Patch(requestBody)


```