---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 29ad565d39b15fbfc5942e7a6df577b394e90d4c
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61086565"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

unifiedRoleEligibilityScheduleId := "unifiedRoleEligibilitySchedule-id"
result, err := graphClient.RoleManagement().Directory().RoleEligibilitySchedulesById(&unifiedRoleEligibilityScheduleId).Get(options)


```