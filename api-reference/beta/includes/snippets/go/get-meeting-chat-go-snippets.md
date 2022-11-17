---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 69f14d77f1f1d2e11b6acdc8dc2c08d7ef46e330
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61021085"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

chatId := "chat-id"
result, err := graphClient.ChatsById(&chatId).Get(options)


```