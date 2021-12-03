---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 06e99f551e002661b3406f576a352741017d1220
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61287481"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

dataPolicyOperationId := "dataPolicyOperation-id"
result, err := graphClient.DataPolicyOperationsById(&dataPolicyOperationId).Get(nil)


```