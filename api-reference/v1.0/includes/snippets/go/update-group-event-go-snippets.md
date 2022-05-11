---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f18f79f0d10268b94dfcc49b96022d02cd3a377f
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65323498"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewEvent()
location := msgraphsdk.NewLocation()
requestBody.SetLocation(location)
displayName := "Conf Room 2"
location.SetDisplayName(&displayName)
groupId := "group-id"
eventId := "event-id"
graphClient.GroupsById(&groupId).Calendar().EventsById(&eventId).Patch(requestBody)


```