---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c5090fd60843ed03822509309e9dc73be107b74c
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61103931"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

messageId := "message-id"
mentionId := "mention-id"
graphClient.Me().MessagesById(&messageId).MentionsById(&mentionId).Delete(options)


```