---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2f705ebfdb995003e0af0a504fdab9515ae80467
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61103656"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

teamId := "team-id"
channelId := "channel-id"
result, err := graphClient.TeamsById(&teamId).ChannelsById(&channelId).FilesFolder().Get(options)


```