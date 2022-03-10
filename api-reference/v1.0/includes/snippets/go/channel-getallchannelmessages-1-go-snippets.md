---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3d750db5a3ca97d0efa1279f6dcce082f5f67061
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411386"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.GetAllMessagesRequestBuilderGetQueryParameters{
    Filter: "lastModifiedDateTime%20gt%202019-11-01T00:00:00Z%20and%20lastModifiedDateTime%20lt%202021-11-01T00:00:00Z",
}
options := &msgraphsdk.GetAllMessagesRequestBuilderGetOptions{
    Q: requestParameters,
}
teamId := "team-id"
result, err := graphClient.TeamsById(&teamId).Channels().GetAllMessages()(team-id).Get(options)


```