---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 28bfdc2962ca5a4c30fe731d292b2f6a68c670e4
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61287083"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

printerId := "printer-id"
result, err := graphClient.Print().PrintersById(&printerId).Shares().Get(nil)


```