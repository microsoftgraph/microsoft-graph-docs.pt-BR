---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6bd06aabb0b80a692ac7cabf9d6fde934265373a
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61286327"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

privilegedRoleAssignmentId := "privilegedRoleAssignment-id"
graphClient.PrivilegedRoleAssignmentsById(&privilegedRoleAssignmentId).Delete(nil)


```