---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2988c4c7d89bcdef96016b10d700d6ef890a3ec2
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61016033"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

teamId := "team-id"
timeOffRequestId := "timeOffRequest-id"
result, err := graphClient.TeamsById(&teamId).Schedule().TimeOffRequestsById(&timeOffRequestId).Get(options)


```