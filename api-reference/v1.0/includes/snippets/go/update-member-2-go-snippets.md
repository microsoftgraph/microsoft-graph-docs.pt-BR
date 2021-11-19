---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ec2516095c84c77e2b5472fa0309bb970aa30d5a
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61103889"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

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