---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b353c30b1c452f2a3c8675e595a6ca1eb6c82395
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65324186"
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
    "user@odata.bind": "https://graph.microsoft.com/v1.0/users('jacob@contoso.com')",
}
teamId := "team-id"
result, err := graphClient.TeamsById(&teamId).Members().Post(requestBody)


```