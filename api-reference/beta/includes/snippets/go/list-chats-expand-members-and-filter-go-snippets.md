---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e22b51eaab35d059b7e38c4ebeea982b49f68ca2
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61087340"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.ChatsRequestBuilderGetQueryParameters{
    Expand: "members",
    Filter: "members/any(o:%20o/displayname%20eq%20'Peter%20Parker')",
}
options := &msgraphsdk.ChatsRequestBuilderGetOptions{
    Q: requestParameters,
}
userId := "user-id"
result, err := graphClient.UsersById(&userId).Chats().Get(options)


```