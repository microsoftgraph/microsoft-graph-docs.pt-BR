---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8c44be6764f61fe957a13e23d4d4014932b7d04d
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65324899"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewConversationMember()
visibleHistoryStartDateTime, err := time.Parse(time.RFC3339, "2019-04-18T23:51:43.255Z")
requestBody.SetVisibleHistoryStartDateTime(&visibleHistoryStartDateTime)
requestBody.SetRoles( []String {
    "owner",
}
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.type": "#microsoft.graph.aadUserConversationMember",
    "user@odata.bind": "https://graph.microsoft.com/beta/users/jacob@contoso.com",
}
chatId := "chat-id"
result, err := graphClient.ChatsById(&chatId).Members().Post(requestBody)


```