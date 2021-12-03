---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0d845b0a6f9780447b40bba576abdf30b75b43ef
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61286176"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

chatId := "chat-id"
conversationMemberId := "conversationMember-id"
result, err := graphClient.ChatsById(&chatId).MembersById(&conversationMemberId).Get(nil)


```