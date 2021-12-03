---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: de49e172e04d90c83a21715689fe12593e65559e
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61287247"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

teamId := "team-id"
timeOffRequestId := "timeOffRequest-id"
result, err := graphClient.TeamsById(&teamId).Schedule().TimeOffRequestsById(&timeOffRequestId).Get(nil)


```