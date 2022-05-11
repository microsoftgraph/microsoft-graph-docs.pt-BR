---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8723104d78d8fd90f389e28b8221617b23e6590a
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65324789"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewChat()
chatType := "oneOnOne"
requestBody.SetChatType(&chatType)
requestBody.SetMembers( []ConversationMember {
    msgraphsdk.NewConversationMember(),
    SetAdditionalData(map[string]interface{}{
        "@odata.type": "#microsoft.graph.aadUserConversationMember",
        "roles":  []String {
            "owner",
        }
        "user@odata.bind": "https://graph.microsoft.com/v1.0/users('jacob@contoso.com')",
    }
    msgraphsdk.NewConversationMember(),
    SetAdditionalData(map[string]interface{}{
        "@odata.type": "#microsoft.graph.aadUserConversationMember",
        "roles":  []String {
            "owner",
        }
        "user@odata.bind": "https://graph.microsoft.com/v1.0/users('alex@contoso.com')",
    }
}
result, err := graphClient.Chats().Post(requestBody)


```