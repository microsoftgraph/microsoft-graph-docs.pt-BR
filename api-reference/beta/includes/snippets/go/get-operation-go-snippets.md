---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4850a712bd980c6cff5f3ad8247c7e4627e6fc67
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61100801"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

userId := "user-id"
longRunningOperationId := "longRunningOperation-id"
result, err := graphClient.UsersById(&userId).Authentication().OperationsById(&longRunningOperationId).Get(options)


```