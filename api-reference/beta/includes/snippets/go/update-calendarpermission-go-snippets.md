---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b0ffa31e932d9b27d53ceced0cc42def62b5e5b7
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65323367"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewCalendarPermission()
role := "write"
requestBody.SetRole(&role)
userId := "user-id"
calendarPermissionId := "calendarPermission-id"
graphClient.UsersById(&userId).Calendar().CalendarPermissionsById(&calendarPermissionId).Patch(requestBody)


```