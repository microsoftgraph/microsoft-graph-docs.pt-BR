---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c37dcf1d8b7049d5b652d906933732e63ca6b8c4
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65325565"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewProjectParticipation()
allowedAudiences := "organization"
requestBody.SetAllowedAudiences(&allowedAudiences)
client := msgraphsdk.NewCompanyDetail()
requestBody.SetClient(client)
department := "Corporate Marketing"
client.SetDepartment(&department)
webUrl := "https://www.contoso.com"
client.SetWebUrl(&webUrl)
projectParticipationId := "projectParticipation-id"
graphClient.Me().Profile().ProjectsById(&projectParticipationId).Patch(requestBody)


```