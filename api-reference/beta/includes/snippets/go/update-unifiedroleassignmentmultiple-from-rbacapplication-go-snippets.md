---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 77ea929eb726104922a932cdc9db42fe4c63314d
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61091792"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewUnifiedRoleAssignmentMultiple()
requestBody.SetPrincipalIds( []String {
    "0aeec2c1-fee7-4e02-b534-6f920d25b300",
    "2d5386a7-732f-44db-9cf8-f82dd2a1c0e0",
}
options := &msgraphsdk.UnifiedRoleAssignmentMultipleRequestBuilderPatchOptions{
    Body: requestBody,
}
unifiedRoleAssignmentMultipleId := "unifiedRoleAssignmentMultiple-id"
graphClient.RoleManagement().DeviceManagement().RoleAssignmentsById(&unifiedRoleAssignmentMultipleId).Patch(options)


```