---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 614569699291569d48b4203367e3deaabbf5e497
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65322291"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

teamId := "team-id"
openShiftId := "openShift-id"
result, err := graphClient.TeamsById(&teamId).Schedule().OpenShiftsById(&openShiftId).Get()


```