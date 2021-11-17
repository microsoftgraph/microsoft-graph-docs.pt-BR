---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 514a22b86dbacf7746019c45e6bd7bb855d79e7e
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "60996697"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

teamId := "team-id"
channelId := "channel-id"
graphClient.TeamsById(&teamId).ChannelsById(&channelId).Patch(options)


```