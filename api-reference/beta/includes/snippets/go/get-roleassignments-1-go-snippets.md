---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b10fb27682b4c0f29a23f015aca3485e96e6b66e
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65324110"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.RoleAssignmentsRequestBuilderGetQueryParameters{
    Filter: "roleDefinitionId%20eq%20'62e90394-69f5-4237-9190-012177145e10'",
    Expand: "principal",
}
options := &msgraphsdk.RoleAssignmentsRequestBuilderGetRequestConfiguration{
    QueryParameters: requestParameters,
}
result, err := graphClient.RoleManagement().Directory().RoleAssignments().GetWithRequestConfigurationAndResponseHandler(options, nil)


```