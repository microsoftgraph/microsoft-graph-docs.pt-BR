---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 91a78823f1e31f7954eeed2a6e4262fec42e7cb5
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65322354"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.RoleManagementPolicyAssignmentsRequestBuilderGetQueryParameters{
    Filter: "scopeId%20eq%20'/'%20and%20scopeType%20eq%20'Directory'",
}
options := &msgraphsdk.RoleManagementPolicyAssignmentsRequestBuilderGetRequestConfiguration{
    QueryParameters: requestParameters,
}
result, err := graphClient.Policies().RoleManagementPolicyAssignments().GetWithRequestConfigurationAndResponseHandler(options, nil)


```