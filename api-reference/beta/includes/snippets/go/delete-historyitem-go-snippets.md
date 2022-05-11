---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 09656524b349bfea8290b52dca0ea4927d7233a6
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65325360"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

userActivityId := "userActivity-id"
activityHistoryItemId := "activityHistoryItem-id"
graphClient.Me().ActivitiesById(&userActivityId).HistoryItemsById(&activityHistoryItemId).Put()


```