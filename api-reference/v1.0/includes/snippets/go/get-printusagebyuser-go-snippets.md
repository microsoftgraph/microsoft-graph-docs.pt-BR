---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 06d1c2ea5b041d2e15f14847bb8f6826ed1da660
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65322148"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

printUsageByUserId := "printUsageByUser-id"
result, err := graphClient.Reports().DailyPrintUsageByUserById(&printUsageByUserId).Get()


```