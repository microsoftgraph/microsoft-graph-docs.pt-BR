---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b2dd196c3d4a249c0cc213e18100b14f3c9274bb
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/05/2022
ms.locfileid: "65204141"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

callId := "call-id"
commsOperationId := "commsOperation-id"
result, err := graphClient.Communications().CallsById(&callId).OperationsById(&commsOperationId).Get(nil)


```