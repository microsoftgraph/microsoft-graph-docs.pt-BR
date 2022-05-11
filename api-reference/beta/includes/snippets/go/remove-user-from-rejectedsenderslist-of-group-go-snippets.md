---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 501c75bedf0366d23fda06acf0cc7bb40fa6fade
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65322494"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.DirectoryObjectRequestBuilderDeleteQueryParameters{
    Id: "https://graph.microsoft.com/beta/users/%7Bid%7D",
}
options := &msgraphsdk.DirectoryObjectRequestBuilderDeleteRequestConfiguration{
    QueryParameters: requestParameters,
}
groupId := "group-id"
directoryObjectId := "directoryObject-id"
graphClient.GroupsById(&groupId).RejectedSendersById(&directoryObjectId).DeleteWithRequestConfigurationAndResponseHandler(options, nil)


```