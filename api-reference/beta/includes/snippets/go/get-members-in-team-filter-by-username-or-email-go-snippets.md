---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 284ee915ec8257b7cd9e3fc0be65d636454a3c49
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61088225"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.MembersRequestBuilderGetQueryParameters{
    Filter: "(microsoft.graph.aadUserConversationMember/displayName%20eq%20'Harry%20Johnson'%20or%20microsoft.graph.aadUserConversationMember/email%20eq%20'admin@M365x987948.OnMicrosoft.com')",
}
options := &msgraphsdk.MembersRequestBuilderGetOptions{
    Q: requestParameters,
}
teamId := "team-id"
result, err := graphClient.TeamsById(&teamId).Members().Get(options)


```