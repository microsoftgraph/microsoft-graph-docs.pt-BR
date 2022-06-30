---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6f8382003ce8373a48df7990e4d425a16186ba76
ms.sourcegitcommit: 54ba08a80db85b9e84813387e8c4416eca44fa8e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/26/2022
ms.locfileid: "65694993"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.PinnedMessagesRequestBuilderGetQueryParameters{
    Expand: "message",
}
options := &msgraphsdk.PinnedMessagesRequestBuilderGetRequestConfiguration{
    QueryParameters: requestParameters,
}
chatId := "chat-id"
result, err := graphClient.ChatsById(&chatId).PinnedMessages().GetWithRequestConfigurationAndResponseHandler(options, nil)


```