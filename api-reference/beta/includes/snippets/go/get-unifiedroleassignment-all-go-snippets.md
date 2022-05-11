---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9d12c2f51e70f87bc66f53e6ddc61b06ae88bbbe
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65322272"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.TransitiveRoleAssignmentsRequestBuilderGetQueryParameters{
    Count: true,
    Filter: "principalId%20eq%20'2c7936bc-3517-40f3-8eda-4806637b6516'",
}
headers := map[string]string{
    "ConsistencyLevel": "eventual"
}
options := &msgraphsdk.TransitiveRoleAssignmentsRequestBuilderGetRequestConfiguration{
    QueryParameters: requestParameters,
    Headers: headers,
}
result, err := graphClient.RoleManagement().Directory().TransitiveRoleAssignments().GetWithRequestConfigurationAndResponseHandler(options, nil)


```