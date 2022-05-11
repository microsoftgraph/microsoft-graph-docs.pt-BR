---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c1c06980a4ef843b7447538ea8fffe9b5120d1b1
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65325056"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

teamId := "team-id"
channelId := "channel-id"
chatMessageId := "chatMessage-id"
chatMessageId1 := "chatMessage-id1"
result, err := graphClient.TeamsById(&teamId).ChannelsById(&channelId).MessagesById(&chatMessageId).RepliesById(&chatMessageId1).HostedContents().Get()


```