---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bf9a55aefec99408ff1a53b33ed4f1d16d70416d
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61286666"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

privilegedRoleAssignmentId := "privilegedRoleAssignment-id"
result, err := graphClient.PrivilegedRoleAssignmentsById(&privilegedRoleAssignmentId).MakeEligible().Post(nil)


```