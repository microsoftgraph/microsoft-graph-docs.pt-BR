---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7081ba4c6872313f8d6d01b6572b5d57d36e5c3f
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65323884"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewOnlineMeeting()
lobbyBypassSettings := msgraphsdk.NewLobbyBypassSettings()
requestBody.SetLobbyBypassSettings(lobbyBypassSettings)
isDialInBypassEnabled := true
lobbyBypassSettings.SetIsDialInBypassEnabled(&isDialInBypassEnabled)
onlineMeetingId := "onlineMeeting-id"
graphClient.Me().OnlineMeetingsById(&onlineMeetingId).Patch(requestBody)


```