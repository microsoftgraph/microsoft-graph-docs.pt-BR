---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 90e8b8ef98e8b65e3b3658f270fc64679a869dc4
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61032029"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

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