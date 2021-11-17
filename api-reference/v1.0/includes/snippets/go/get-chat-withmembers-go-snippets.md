---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 46fa82681a88acaf02cbe741e2efaa889d2ac646
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "60996572"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestParameters := &msgraphsdk.ChatRequestBuilderGetQueryParameters{
    Expand: "members",
}
options := &msgraphsdk.ChatRequestBuilderGetOptions{
    Q: requestParameters,
}
chatId := "chat-id"
result, err := graphClient.ChatsById(&chatId).Get(options)


```