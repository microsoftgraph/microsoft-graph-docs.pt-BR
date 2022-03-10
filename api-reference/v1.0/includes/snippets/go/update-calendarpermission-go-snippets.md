---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b38f7ca94780725ddb160f1333c5f1ec0d4c4076
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411136"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewCalendarPermission()
role := "write"
requestBody.SetRole(&role)
options := &msgraphsdk.CalendarPermissionRequestBuilderPatchOptions{
    Body: requestBody,
}
userId := "user-id"
calendarPermissionId := "calendarPermission-id"
result, err := graphClient.UsersById(&userId).Calendar().CalendarPermissionsById(&calendarPermissionId).Patch(options)


```