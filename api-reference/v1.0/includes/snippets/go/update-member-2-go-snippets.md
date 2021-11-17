---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0a77eb52e0e785ec44deda976364fb4d99ad5045
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61018945"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewConversationMember()
requestBody.SetRoles( []String {
    "owner",
}
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.type": "#microsoft.graph.aadUserConversationMember",
}
options := &msgraphsdk.ConversationMemberRequestBuilderPatchOptions{
    Body: requestBody,
}
teamId := "team-id"
conversationMemberId := "conversationMember-id"
graphClient.TeamsById(&teamId).MembersById(&conversationMemberId).Patch(options)


```