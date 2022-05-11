---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 00acb4c004c05c5636581ede9b2b98a0a73062d7
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65322327"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.RoleAssignmentsRequestBuilderGetQueryParameters{
    Filter: "appScopeId%20eq%20'/AccessPackageCatalog/4cee616b-fdf9-4890-9d10-955e0ccb12bc'",
    Expand: "principal",
}
options := &msgraphsdk.RoleAssignmentsRequestBuilderGetRequestConfiguration{
    QueryParameters: requestParameters,
}
result, err := graphClient.RoleManagement().EntitlementManagement().RoleAssignments().GetWithRequestConfigurationAndResponseHandler(options, nil)


```