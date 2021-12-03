---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 707f21f4cd2ea8dcd76b8aca2b3d507f0b4b4c5f
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61287237"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

messageId := "message-id"
attachmentId := "attachment-id"
result, err := graphClient.Me().MessagesById(&messageId).AttachmentsById(&attachmentId).Get(nil)


```