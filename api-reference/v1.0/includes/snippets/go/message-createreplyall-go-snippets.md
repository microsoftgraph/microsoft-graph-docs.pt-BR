---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 55e59cc413e57d5ee8675ddd9fbbe69871908643
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65324485"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

messageId := "message-id"
result, err := graphClient.Me().MessagesById(&messageId).CreateReplyAll(message-id).Post()


```