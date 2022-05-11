---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b6e57cef5a346295ceb21f1a5fffa5a17b0fd983
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65324486"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

messageId := "message-id"
result, err := graphClient.Me().MessagesById(&messageId).CreateForward(message-id).Post()


```