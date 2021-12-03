---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 51ea2563699da4c0d54bc98822c533a227f2851b
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61286313"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

userId := "user-id"
chatId := "chat-id"
result, err := graphClient.UsersById(&userId).ChatsById(&chatId).Get(nil)


```