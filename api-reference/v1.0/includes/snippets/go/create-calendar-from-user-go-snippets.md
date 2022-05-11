---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 45c695b85cb3fd44ce4179007051e2c06f95074e
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65323580"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewCalendar()
name := "Volunteer"
requestBody.SetName(&name)
result, err := graphClient.Me().Calendars().Post(requestBody)


```