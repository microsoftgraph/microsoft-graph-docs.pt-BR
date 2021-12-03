---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 46d13cc7b1a1f63af5c86b96c7fead8898e04d3f
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61287003"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

userActivityId := "userActivity-id"
activityHistoryItemId := "activityHistoryItem-id"
graphClient.Me().ActivitiesById(&userActivityId).HistoryItemsById(&activityHistoryItemId).Put(nil)


```