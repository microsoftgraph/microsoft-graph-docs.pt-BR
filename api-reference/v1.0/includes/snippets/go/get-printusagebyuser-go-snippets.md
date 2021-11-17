---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c75d7ebaccee72571216837db5b63a00e16682c7
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61032862"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

printUsageByUserId := "printUsageByUser-id"
result, err := graphClient.Reports().DailyPrintUsageByUserById(&printUsageByUserId).Get(options)


```