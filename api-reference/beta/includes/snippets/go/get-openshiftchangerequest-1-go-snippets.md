---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 16be6a2e62c1256f9e008610c17d3c2a7ee9e280
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61286001"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

teamId := "team-id"
openShiftChangeRequestId := "openShiftChangeRequest-id"
result, err := graphClient.TeamsById(&teamId).Schedule().OpenShiftChangeRequestsById(&openShiftChangeRequestId).Get(nil)


```