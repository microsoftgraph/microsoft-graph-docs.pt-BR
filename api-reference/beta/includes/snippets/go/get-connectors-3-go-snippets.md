---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b8d0307a042b1dba2e958e3948af59109a1791e4
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61287358"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

printerId := "printer-id"
result, err := graphClient.Print().PrintersById(&printerId).Connectors().Get(nil)


```