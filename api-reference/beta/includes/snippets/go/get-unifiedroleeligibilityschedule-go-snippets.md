---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 577e635963e8a8cb2fccce4881cf2418e88febdc
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61287023"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

unifiedRoleEligibilityScheduleId := "unifiedRoleEligibilitySchedule-id"
result, err := graphClient.RoleManagement().Directory().RoleEligibilitySchedulesById(&unifiedRoleEligibilityScheduleId).Get(nil)


```