---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6acabb1fb88029bd961a5b1db73d887038cd53c1
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411013"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

messageId := "message-id"
graphClient.Me().MessagesById(&messageId).Unsubscribe(message-id).Post(nil)


```