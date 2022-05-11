---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0256d35cb96e92466ffae8dde85ad5945a246a3f
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65324751"
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
teamId := "team-id"
result, err := graphClient.TeamsById(&teamId).Schedule().TimeOffReasons().Post(requestBody)


```