---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e11e4392638e5ebe45d2e8c9d37a87ae2daf1c7b
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61286917"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

printUsageByPrinterId := "printUsageByPrinter-id"
result, err := graphClient.Reports().DailyPrintUsageByPrinterById(&printUsageByPrinterId).Get(nil)


```