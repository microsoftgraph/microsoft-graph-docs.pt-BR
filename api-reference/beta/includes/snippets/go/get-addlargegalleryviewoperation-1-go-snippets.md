---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d6683f5b72dd1e0c23163ed0b7db50412ec45163
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65322568"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

callId := "call-id"
commsOperationId := "commsOperation-id"
result, err := graphClient.Communications().CallsById(&callId).OperationsById(&commsOperationId).Get()


```