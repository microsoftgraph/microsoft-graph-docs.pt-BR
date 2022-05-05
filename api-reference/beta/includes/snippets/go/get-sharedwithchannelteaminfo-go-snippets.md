---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 30eefc9093503966337474105557c36864dd357e
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/05/2022
ms.locfileid: "65212470"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

teamId := "team-id"
channelId := "channel-id"
sharedWithChannelTeamInfoId := "sharedWithChannelTeamInfo-id"
result, err := graphClient.TeamsById(&teamId).ChannelsById(&channelId).SharedWithTeamsById(&sharedWithChannelTeamInfoId).Get(nil)


```