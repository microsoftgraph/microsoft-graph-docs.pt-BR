---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a90d8925e63ce82e93a2579b453e0dda70f90342
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61005889"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

userId := "user-id"
appRoleAssignmentId := "appRoleAssignment-id"
graphClient.UsersById(&userId).AppRoleAssignmentsById(&appRoleAssignmentId).Delete(options)


```