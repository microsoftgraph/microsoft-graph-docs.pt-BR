---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 671fdecfecb988b52f6d8850d9c6abe2277135e1
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65324915"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewMessage()
isRead := true
requestBody.SetIsRead(&isRead)
messageId := "message-id"
graphClient.Me().MessagesById(&messageId).Patch(requestBody)


```