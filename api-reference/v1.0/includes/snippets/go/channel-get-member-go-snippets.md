---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 13b4ddf263c94dc8c4ee9a96ed713a7e8f58b0ff
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61100862"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

teamId := "team-id"
channelId := "channel-id"
conversationMemberId := "conversationMember-id"
result, err := graphClient.TeamsById(&teamId).ChannelsById(&channelId).MembersById(&conversationMemberId).Get(options)


```