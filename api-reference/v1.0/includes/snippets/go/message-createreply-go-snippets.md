---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 70478a071541edb121d30b78d236edaed3318bc4
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411509"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

messageId := "message-id"
result, err := graphClient.Me().MessagesById(&messageId).CreateReply(message-id).Post(nil)


```