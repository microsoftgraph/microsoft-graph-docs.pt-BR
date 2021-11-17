---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7076bc29081b0151b82c06dfd9481ae03c7ac4fd
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61017160"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

unifiedRoleAssignmentScheduleId := "unifiedRoleAssignmentSchedule-id"
result, err := graphClient.RoleManagement().Directory().RoleAssignmentSchedulesById(&unifiedRoleAssignmentScheduleId).Get(options)


```