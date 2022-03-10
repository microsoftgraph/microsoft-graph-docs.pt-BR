---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1753918395b98d33295da21ef4930094bdc1a98e
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2022
ms.locfileid: "63410547"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

chatId := "chat-id"
conversationMemberId := "conversationMember-id"
result, err := graphClient.ChatsById(&chatId).MembersById(&conversationMemberId).Delete(nil)


```