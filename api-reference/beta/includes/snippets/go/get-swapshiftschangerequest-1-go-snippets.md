---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b77a9a1f67ccc7131e5223a5c00a090f3e860f81
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65322456"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

teamId := "team-id"
swapShiftsChangeRequestId := "swapShiftsChangeRequest-id"
result, err := graphClient.TeamsById(&teamId).Schedule().SwapShiftsChangeRequestsById(&swapShiftsChangeRequestId).Get()


```