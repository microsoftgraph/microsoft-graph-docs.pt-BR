---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 98c00d400f737df62adbdd065275f5eaaa64a9fe
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/15/2022
ms.locfileid: "66092566"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

privilegedAccessId := "privilegedAccess-id"
governanceRoleAssignmentRequestId := "governanceRoleAssignmentRequest-id"
graphClient.PrivilegedAccessById(&privilegedAccessId).RoleAssignmentRequestsById(&governanceRoleAssignmentRequestId).Cancel(privilegedAccess-id, governanceRoleAssignmentRequest-id).Post()


```