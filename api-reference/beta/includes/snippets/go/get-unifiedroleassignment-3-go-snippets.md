---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2893dcf62a44833eedd93f072a7589d822cfe499
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65323200"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.UnifiedRoleAssignmentMultipleRequestBuilderGetQueryParameters{
    Expand: "roleDefinition",
}
options := &msgraphsdk.UnifiedRoleAssignmentMultipleRequestBuilderGetRequestConfiguration{
    QueryParameters: requestParameters,
}
unifiedRoleAssignmentMultipleId := "unifiedRoleAssignmentMultiple-id"
result, err := graphClient.RoleManagement().CloudPC().RoleAssignmentsById(&unifiedRoleAssignmentMultipleId).GetWithRequestConfigurationAndResponseHandler(options, nil)


```