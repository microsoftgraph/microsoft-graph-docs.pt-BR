---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bfc42363a871e379d79394d4dcf6e2dea11d5489
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61094226"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

teamId := "team-id"
openShiftChangeRequestId := "openShiftChangeRequest-id"
result, err := graphClient.TeamsById(&teamId).Schedule().OpenShiftChangeRequestsById(&openShiftChangeRequestId).Get(options)


```