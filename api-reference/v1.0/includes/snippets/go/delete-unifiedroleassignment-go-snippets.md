---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c97bf06e7b4c954ee70f1e26f9d114927f3c6f31
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65322135"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

unifiedRoleAssignmentId := "unifiedRoleAssignment-id"
graphClient.RoleManagement().Directory().RoleAssignmentsById(&unifiedRoleAssignmentId).Delete()


```