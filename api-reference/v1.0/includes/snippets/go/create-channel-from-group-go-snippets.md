---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c0f390ba3b4c1c208aae88e0b1ea76bd786ea8ff
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65316132"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewChannel()
displayName := "Architecture Discussion"
requestBody.SetDisplayName(&displayName)
description := "This channel is where we debate all future architecture plans"
requestBody.SetDescription(&description)
membershipType := "standard"
requestBody.SetMembershipType(&membershipType)
teamId := "team-id"
result, err := graphClient.TeamsById(&teamId).Channels().Post(requestBody)


```