---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 589133132c72515dfa412da372f697fb91096380
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61099684"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

teamId := "team-id"
timeOffReasonId := "timeOffReason-id"
graphClient.TeamsById(&teamId).Schedule().TimeOffReasonsById(&timeOffReasonId).Delete(options)


```