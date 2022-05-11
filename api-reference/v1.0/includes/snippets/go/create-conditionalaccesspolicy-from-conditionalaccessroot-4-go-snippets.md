---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c4ce4d51a4a584e18b7a5e5c6b74d1b96bfbff79
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65323516"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewConditionalAccessPolicy()
displayName := "Require MFA to EXO from non-compliant devices."
requestBody.SetDisplayName(&displayName)
state := "enabled"
requestBody.SetState(&state)
conditions := msgraphsdk.NewConditionalAccessConditionSet()
requestBody.SetConditions(conditions)
applications := msgraphsdk.NewConditionalAccessApplications()
conditions.SetApplications(applications)
applications.SetIncludeApplications( []String {
    "00000002-0000-0ff1-ce00-000000000000",
}
users := msgraphsdk.NewConditionalAccessUsers()
conditions.SetUsers(users)
users.SetIncludeGroups( []String {
    "ba8e7ded-8b0f-4836-ba06-8ff1ecc5c8ba",
}
grantControls := msgraphsdk.NewConditionalAccessGrantControls()
requestBody.SetGrantControls(grantControls)
operator := "OR"
grantControls.SetOperator(&operator)
grantControls.SetBuiltInControls( []ConditionalAccessGrantControl {
    "mfa",
}
result, err := graphClient.Identity().ConditionalAccess().Policies().Post(requestBody)


```