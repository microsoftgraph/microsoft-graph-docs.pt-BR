---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 36831e346c53d561c9df4d47a857a9de47a699d8
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65323991"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewChannel()
displayName := "UpdateChannelModeration"
requestBody.SetDisplayName(&displayName)
description := "Update channel moderation."
requestBody.SetDescription(&description)
moderationSettings := msgraphsdk.NewChannelModerationSettings()
requestBody.SetModerationSettings(moderationSettings)
userNewMessageRestriction := "moderators"
moderationSettings.SetUserNewMessageRestriction(&userNewMessageRestriction)
replyRestriction := "everyone"
moderationSettings.SetReplyRestriction(&replyRestriction)
allowNewMessageFromBots := true
moderationSettings.SetAllowNewMessageFromBots(&allowNewMessageFromBots)
allowNewMessageFromConnectors := true
moderationSettings.SetAllowNewMessageFromConnectors(&allowNewMessageFromConnectors)
teamId := "team-id"
channelId := "channel-id"
graphClient.TeamsById(&teamId).ChannelsById(&channelId).Patch(requestBody)


```