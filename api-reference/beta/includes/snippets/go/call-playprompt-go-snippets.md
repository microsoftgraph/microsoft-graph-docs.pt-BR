---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2fb2a06719d24508c7cca4ec1159c20af2105404
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61286199"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

callId := "call-id"
result, err := graphClient.Communications().CallsById(&callId).PlayPrompt().Post(nil)


```