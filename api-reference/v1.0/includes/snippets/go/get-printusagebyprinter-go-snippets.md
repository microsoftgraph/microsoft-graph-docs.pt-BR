---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 17aea5d755f92e84e571e644e1f5959f3c8ed2a9
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61084513"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

printUsageByPrinterId := "printUsageByPrinter-id"
result, err := graphClient.Reports().DailyPrintUsageByPrinterById(&printUsageByPrinterId).Get(options)


```