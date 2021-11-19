---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b0ae0c677dfb7a0009ef8f180860b05726323d87
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61096899"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

printerId := "printer-id"
result, err := graphClient.Print().PrintersById(&printerId).TaskTriggers().Get(options)


```