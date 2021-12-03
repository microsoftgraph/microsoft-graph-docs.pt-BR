---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2c69e82e43ce7d1abc5a8f6eff6f4bfbca391fcf
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61287349"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

unifiedRoleAssignmentScheduleInstanceId := "unifiedRoleAssignmentScheduleInstance-id"
result, err := graphClient.RoleManagement().Directory().RoleAssignmentScheduleInstancesById(&unifiedRoleAssignmentScheduleInstanceId).Get(nil)


```