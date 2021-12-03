---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4c855f71b749675079c63715c6a271b60f92f309
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61287200"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

unifiedRoleAssignmentScheduleId := "unifiedRoleAssignmentSchedule-id"
result, err := graphClient.RoleManagement().Directory().RoleAssignmentSchedulesById(&unifiedRoleAssignmentScheduleId).Get(nil)


```