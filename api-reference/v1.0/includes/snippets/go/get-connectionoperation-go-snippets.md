---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a7b8cca794e6d63d63b7b9dcbf1ec0e873c4dda3
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65322769"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

externalConnectionId := "externalConnection-id"
connectionOperationId := "connectionOperation-id"
result, err := graphClient.External().ConnectionsById(&externalConnectionId).OperationsById(&connectionOperationId).Get()


```