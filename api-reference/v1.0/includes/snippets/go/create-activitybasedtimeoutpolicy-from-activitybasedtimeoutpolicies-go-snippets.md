---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: be1ff1e5e56142a4d8f9b05194d0df38f9341b57
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61100034"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewActivityBasedTimeoutPolicy()
requestBody.SetDefinition( []String {
    "definition-value",
}
displayName := "displayName-value"
requestBody.SetDisplayName(&displayName)
isOrganizationDefault := true
requestBody.SetIsOrganizationDefault(&isOrganizationDefault)
options := &msgraphsdk.ActivityBasedTimeoutPoliciesRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Policies().ActivityBasedTimeoutPolicies().Post(options)


```