---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e9ce43a3b67c1cad6ccb9f00336f37fb2fc04259
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61019617"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

privilegedRoleAssignmentId := "privilegedRoleAssignment-id"
result, err := graphClient.PrivilegedRoleAssignmentsById(&privilegedRoleAssignmentId).Get(options)


```