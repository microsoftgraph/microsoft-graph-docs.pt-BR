---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 665084850445a2cf35f2a11cb86ec101a900e0b6
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61100365"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

privilegedRoleAssignmentId := "privilegedRoleAssignment-id"
result, err := graphClient.PrivilegedRoleAssignmentsById(&privilegedRoleAssignmentId).MakeEligible().Post(options)


```