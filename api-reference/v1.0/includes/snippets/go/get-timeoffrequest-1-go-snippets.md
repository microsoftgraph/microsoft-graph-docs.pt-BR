---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 543c57a2bd7bd761b323e3f3a90715fa9b5877b4
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65324177"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

teamId := "team-id"
timeOffRequestId := "timeOffRequest-id"
result, err := graphClient.TeamsById(&teamId).Schedule().TimeOffRequestsById(&timeOffRequestId).Get()


```