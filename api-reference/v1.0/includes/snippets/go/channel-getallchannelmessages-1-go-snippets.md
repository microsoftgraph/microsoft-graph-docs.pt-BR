---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 25107ecc9d43ba8d72992032fe1ffe64fd183659
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62137586"
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
result, err := graphClient.TeamsById(&teamId).Channels().GetAllMessages()().Get(options)


```