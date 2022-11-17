---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b0a184d95cedf908a5e1a4cb5bd6616e53dd016b
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "60996573"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

userId := "user-id"
chatId := "chat-id"
result, err := graphClient.UsersById(&userId).ChatsById(&chatId).Get(options)


```