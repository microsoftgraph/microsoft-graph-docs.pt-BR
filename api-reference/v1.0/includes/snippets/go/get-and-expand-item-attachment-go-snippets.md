---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fe8c9fc64a152fbc332c180ff43dbe8f8c373aac
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61099392"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.AttachmentRequestBuilderGetQueryParameters{
    Expand: "microsoft.graph.itemattachment/item",
}
options := &msgraphsdk.AttachmentRequestBuilderGetOptions{
    Q: requestParameters,
}
messageId := "message-id"
attachmentId := "attachment-id"
result, err := graphClient.Me().MessagesById(&messageId).AttachmentsById(&attachmentId).Get(options)


```