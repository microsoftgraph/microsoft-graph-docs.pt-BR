---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2931a61fe4a6496267320f5e2a4a51cc51c28cc2
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65324173"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

unifiedRoleEligibilityScheduleInstanceId := "unifiedRoleEligibilityScheduleInstance-id"
result, err := graphClient.RoleManagement().Directory().RoleEligibilityScheduleInstancesById(&unifiedRoleEligibilityScheduleInstanceId).Get()


```