---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b6b850e39dab2cf0c9e50d543eebbeb41e94f65e
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65325496"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewAttachmentItemRequestBody()
attachmentItem := msgraphsdk.NewAttachmentItem()
requestBody.SetAttachmentItem(attachmentItem)
attachmentType := "file"
attachmentItem.SetAttachmentType(&attachmentType)
name := "flower"
attachmentItem.SetName(&name)
size := int64(3483322)
attachmentItem.SetSize(&size)
messageId := "message-id"
result, err := graphClient.Me().MessagesById(&messageId).Attachments().CreateUploadSession(message-id).Post(requestBody)


```