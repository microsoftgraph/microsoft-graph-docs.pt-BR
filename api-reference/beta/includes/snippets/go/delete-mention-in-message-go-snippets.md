---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 322de593a921e83c5218d529b8cf4bacd356fb19
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "60980842"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

messageId := "message-id"
mentionId := "mention-id"
graphClient.Me().MessagesById(&messageId).MentionsById(&mentionId).Delete(options)


```