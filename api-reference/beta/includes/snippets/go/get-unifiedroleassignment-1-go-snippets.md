---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a269f9bc813774c86a9a171304fb2977922bee72
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65324044"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

unifiedRoleAssignmentId := "unifiedRoleAssignment-id"
result, err := graphClient.RoleManagement().Directory().RoleAssignmentsById(&unifiedRoleAssignmentId).Get()


```