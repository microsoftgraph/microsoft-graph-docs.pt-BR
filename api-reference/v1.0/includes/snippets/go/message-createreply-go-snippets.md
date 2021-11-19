---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b62e8579100cb9c52de158e65f2bd6acad0b054e
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61098861"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

messageId := "message-id"
result, err := graphClient.Me().MessagesById(&messageId).CreateReply().Post(options)


```