---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: dda200c5ea16774d89b09fcd63e743d58a900bc7
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61028330"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestParameters := &msgraphsdk.MessageRequestBuilderGetQueryParameters{
    Select: "subject,body,bodyPreview,uniqueBody",
}
headers := map[string]string{
    "Prefer": "outlook.body-content-type="text""
}
options := &msgraphsdk.MessageRequestBuilderGetOptions{
    Q: requestParameters,
    H: headers,
}
messageId := "message-id"
result, err := graphClient.Me().MessagesById(&messageId).Get(options)


```