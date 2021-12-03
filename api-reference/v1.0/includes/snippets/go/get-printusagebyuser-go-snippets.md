---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 29fd7f42479809bbbd470390bfbb06ff0d709319
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61287451"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

printUsageByUserId := "printUsageByUser-id"
result, err := graphClient.Reports().DailyPrintUsageByUserById(&printUsageByUserId).Get(nil)


```