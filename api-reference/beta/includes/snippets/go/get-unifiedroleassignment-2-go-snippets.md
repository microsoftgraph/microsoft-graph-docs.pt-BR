---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e5ba6913b0cbf0f1c31abe3bfd46d4f58fb309d1
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65324045"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.UnifiedRoleAssignmentRequestBuilderGetQueryParameters{
    Expand: "roleDefinition",
}
options := &msgraphsdk.UnifiedRoleAssignmentRequestBuilderGetRequestConfiguration{
    QueryParameters: requestParameters,
}
unifiedRoleAssignmentId := "unifiedRoleAssignment-id"
result, err := graphClient.RoleManagement().Directory().RoleAssignmentsById(&unifiedRoleAssignmentId).GetWithRequestConfigurationAndResponseHandler(options, nil)


```