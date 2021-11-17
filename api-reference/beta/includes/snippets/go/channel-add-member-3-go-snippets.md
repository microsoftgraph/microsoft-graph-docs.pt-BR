---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0d59e860e9a226002ce64710217372dcf02d1d6d
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61026891"
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
    "user@odata.bind": "https://graph.microsoft.com/beta/users('jacob@contoso.com')",
}
options := &msgraphsdk.MembersRequestBuilderPostOptions{
    Body: requestBody,
}
teamId := "team-id"
channelId := "channel-id"
result, err := graphClient.TeamsById(&teamId).ChannelsById(&channelId).Members().Post(options)


```