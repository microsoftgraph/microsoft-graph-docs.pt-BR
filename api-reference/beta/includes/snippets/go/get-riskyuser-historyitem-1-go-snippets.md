---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 12a7e8be74580d195cc2b58a8c1be3645dc73329
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61098781"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

riskyUserId := "riskyUser-id"
riskyUserHistoryItemId := "riskyUserHistoryItem-id"
result, err := graphClient.RiskyUsersById(&riskyUserId).HistoryById(&riskyUserHistoryItemId).Get(options)


```