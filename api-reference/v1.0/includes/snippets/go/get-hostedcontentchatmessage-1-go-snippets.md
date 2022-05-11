---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 531a2d7db4aa63b6ce9e3051fbdfcae239e667fc
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65323772"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

chatId := "chat-id"
chatMessageId := "chatMessage-id"
chatMessageHostedContentId := "chatMessageHostedContent-id"
result, err := graphClient.ChatsById(&chatId).MessagesById(&chatMessageId).HostedContentsById(&chatMessageHostedContentId).Get()


```