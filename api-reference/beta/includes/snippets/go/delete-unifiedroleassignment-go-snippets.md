---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cd7039f467052bc33e0d442278e09f622e23243a
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61287286"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

unifiedRoleAssignmentId := "unifiedRoleAssignment-id"
graphClient.RoleManagement().Directory().RoleAssignmentsById(&unifiedRoleAssignmentId).Delete(nil)


```