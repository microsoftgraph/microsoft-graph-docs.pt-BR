---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 064378f67889c0c86fa2a93f21c1de15560db0f3
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65324156"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

teamId := "team-id"
channelId := "channel-id"
graphClient.TeamsById(&teamId).ChannelsById(&channelId).CompleteMigration(team-id, channel-id).Post()


```