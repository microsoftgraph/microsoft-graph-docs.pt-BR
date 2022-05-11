---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a61cb0c8d884b739ddb2cf332a93eadc86b9d51b
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65323429"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

chatId := "chat-id"
teamsAsyncOperationId := "teamsAsyncOperation-id"
result, err := graphClient.ChatsById(&chatId).OperationsById(&teamsAsyncOperationId).Get()


```