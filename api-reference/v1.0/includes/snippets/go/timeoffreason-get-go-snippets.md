---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bdba7941103519e57f6f42f9effddd5d5e30a29f
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61286509"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

teamId := "team-id"
timeOffReasonId := "timeOffReason-id"
result, err := graphClient.TeamsById(&teamId).Schedule().TimeOffReasonsById(&timeOffReasonId).Get(nil)


```