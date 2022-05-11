---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 309175d2b9c29d8c9f117655666e7931f71ade72
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65323185"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewChat()
topic := "Group chat title update"
requestBody.SetTopic(&topic)
chatId := "chat-id"
graphClient.ChatsById(&chatId).Patch(requestBody)


```