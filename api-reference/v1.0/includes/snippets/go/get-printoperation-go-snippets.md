---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 63f6a32d3a4a0826e7253f014a1d6b180f2f7f3a
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65322850"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

printOperationId := "printOperation-id"
result, err := graphClient.Print().OperationsById(&printOperationId).Get()


```