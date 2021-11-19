---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c8da801ea77220df55ed1f1bdf84fd5bf134c63b
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61092085"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewTimeOffReason()
displayName := "Vacation"
requestBody.SetDisplayName(&displayName)
iconType := "plane"
requestBody.SetIconType(&iconType)
isActive := true
requestBody.SetIsActive(&isActive)
options := &msgraphsdk.TimeOffReasonsRequestBuilderPostOptions{
    Body: requestBody,
}
teamId := "team-id"
result, err := graphClient.TeamsById(&teamId).Schedule().TimeOffReasons().Post(options)


```