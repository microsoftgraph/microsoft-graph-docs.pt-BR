---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ff5d6a40571a00dc615880ff9f5a0cc350e5607e
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65322987"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

teamId := "team-id"
timeOffReasonId := "timeOffReason-id"
result, err := graphClient.TeamsById(&teamId).Schedule().TimeOffReasonsById(&timeOffReasonId).Get()


```