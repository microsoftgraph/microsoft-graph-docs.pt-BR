---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 15fc4310074dbe03f5f0811b5303990c96786123
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65325422"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewTeamworkTag()
displayName := "Finance"
requestBody.SetDisplayName(&displayName)
teamId := "team-id"
teamworkTagId := "teamworkTag-id"
graphClient.TeamsById(&teamId).TagsById(&teamworkTagId).Patch(requestBody)


```