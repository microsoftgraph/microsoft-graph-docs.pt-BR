---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 90aa977553bfadc6c37236cfc4a099ae3bf8452a
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65324301"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.ChatsRequestBuilderGetQueryParameters{
    Expand: "members",
    Filter: "members/any(o:%20o/displayname%20eq%20'Peter%20Parker')",
}
options := &msgraphsdk.ChatsRequestBuilderGetRequestConfiguration{
    QueryParameters: requestParameters,
}
userId := "user-id"
result, err := graphClient.UsersById(&userId).Chats().GetWithRequestConfigurationAndResponseHandler(options, nil)


```