---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: aa4612fa115062a6c5112d5387d67b4a9bed53c8
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61033382"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestParameters := &msgraphsdk.MessagesRequestBuilderGetQueryParameters{
    Filter: "MentionsPreview/IsMentioned%20eq%20true",
    Select: "Subject,Sender,ReceivedDateTime,MentionsPreview",
}
options := &msgraphsdk.MessagesRequestBuilderGetOptions{
    Q: requestParameters,
}
result, err := graphClient.Me().Messages().Get(options)


```