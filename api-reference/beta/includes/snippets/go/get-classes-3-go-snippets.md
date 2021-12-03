---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 40d8517a3645a3bd89413157824a7e04652ebe39
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61286050"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Education().Me().Classes().Get(nil)


```