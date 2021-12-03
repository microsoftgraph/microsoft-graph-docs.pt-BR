---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8d54acc9950b75acb439ef952ee098d3abb4c213
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61286756"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

unifiedRoleManagementPolicyAssignmentId := "unifiedRoleManagementPolicyAssignment-id"
result, err := graphClient.Policies().RoleManagementPolicyAssignmentsById(&unifiedRoleManagementPolicyAssignmentId).Get(nil)


```