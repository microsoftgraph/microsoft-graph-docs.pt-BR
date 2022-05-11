---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ef6c9dbc1a58311608d363a0b5fa83a3af7d3a14
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65323964"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

messageId := "message-id"
graphClient.Me().MessagesById(&messageId).Send(message-id).Post()


```