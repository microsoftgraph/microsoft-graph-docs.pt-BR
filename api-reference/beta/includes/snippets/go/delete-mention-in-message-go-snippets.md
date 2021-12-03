---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ff3499e2b697a9a1c54d65d6d715ad0a8315a48c
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61286042"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

messageId := "message-id"
mentionId := "mention-id"
graphClient.Me().MessagesById(&messageId).MentionsById(&mentionId).Delete(nil)


```