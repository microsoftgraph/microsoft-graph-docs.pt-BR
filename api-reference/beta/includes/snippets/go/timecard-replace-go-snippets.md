---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a6e1a31810d09f8171559bef915f7996b362025c
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65322196"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetAdditionalData(map[string]interface{}{
    "userId": "70e47528-2fae-42b5-9d8e-ee73ccd90603",
    "state": "clockedOut",
    "confirmedBy": "None",
    "notes": nil,
    "breaks":  []Object {
    }
}
teamId := "team-id"
timeCardId := "timeCard-id"
graphClient.TeamsById(&teamId).Schedule().TimeCardsById(&timeCardId).Put(requestBody)


```