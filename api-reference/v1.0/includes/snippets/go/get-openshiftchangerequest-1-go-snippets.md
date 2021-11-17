---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 95b5f5e22fbf7f3fdfd749a3f5a72464cf342e82
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "60984483"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

teamId := "team-id"
openShiftChangeRequestId := "openShiftChangeRequest-id"
result, err := graphClient.TeamsById(&teamId).Schedule().OpenShiftChangeRequestsById(&openShiftChangeRequestId).Get(options)


```