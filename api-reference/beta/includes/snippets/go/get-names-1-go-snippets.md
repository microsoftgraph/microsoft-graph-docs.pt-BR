---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0bc0ca8977df3ede10d2ac3077731f7fc0046055
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61287333"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Me().Profile().Names().Get(nil)


```