---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f54c78d20fc6b1c4ebad767030e34ea8a49982f0
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65324449"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

teamId := "team-id"
timeOffRequestId := "timeOffRequest-id"
graphClient.TeamsById(&teamId).Schedule().TimeOffRequestsById(&timeOffRequestId).Delete()


```