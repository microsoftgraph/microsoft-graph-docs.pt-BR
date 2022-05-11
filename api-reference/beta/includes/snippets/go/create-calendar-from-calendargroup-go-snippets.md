---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7cb54bc637c0336956981ffd2fc7cb59742d1155
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65323920"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewCalendar()
name := "Marketing calendar"
requestBody.SetName(&name)
calendarGroupId := "calendarGroup-id"
result, err := graphClient.Me().CalendarGroupsById(&calendarGroupId).Calendars().Post(requestBody)


```