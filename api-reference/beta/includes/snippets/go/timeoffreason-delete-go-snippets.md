---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 36b2775dfd8cf41d73761e28324e1f6a53008524
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2022
ms.locfileid: "63410655"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

teamId := "team-id"
timeOffReasonId := "timeOffReason-id"
result, err := graphClient.TeamsById(&teamId).Schedule().TimeOffReasonsById(&timeOffReasonId).Delete(nil)


```