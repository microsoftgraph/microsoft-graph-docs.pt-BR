---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9c8cf596895218a3fc162d6b3fd79a70cc44771c
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65323198"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewUnifiedRoleEligibilityScheduleRequest()
action := "AdminAssign"
requestBody.SetAction(&action)
justification := "Assign User Admin eligibility to IT Helpdesk (User) group"
requestBody.SetJustification(&justification)
roleDefinitionId := "fdd7a751-b60b-444a-984c-02652fe8fa1c"
requestBody.SetRoleDefinitionId(&roleDefinitionId)
directoryScopeId := "/"
requestBody.SetDirectoryScopeId(&directoryScopeId)
principalId := "07706ff1-46c7-4847-ae33-3003830675a1"
requestBody.SetPrincipalId(&principalId)
scheduleInfo := msgraphsdk.NewRequestSchedule()
requestBody.SetScheduleInfo(scheduleInfo)
startDateTime, err := time.Parse(time.RFC3339, "2021-07-01T00:00:00Z")
scheduleInfo.SetStartDateTime(&startDateTime)
expiration := msgraphsdk.NewExpirationPattern()
scheduleInfo.SetExpiration(expiration)
endDateTime, err := time.Parse(time.RFC3339, "2022-06-30T00:00:00Z")
expiration.SetEndDateTime(&endDateTime)
type := "AfterDateTime"
expiration.SetType(&type)
result, err := graphClient.RoleManagement().Directory().RoleEligibilityScheduleRequests().Post(requestBody)


```