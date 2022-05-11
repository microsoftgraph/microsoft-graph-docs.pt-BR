---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c7b4cddd719540380d769356eaf75183d2153922
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65325292"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.AccessPackageAssignmentRequestsRequestBuilderGetQueryParameters{
    Expand: "requestor($expand=connectedOrganization)",
    Filter: "(requestState%20eq%20'PendingApproval')",
}
options := &msgraphsdk.AccessPackageAssignmentRequestsRequestBuilderGetRequestConfiguration{
    QueryParameters: requestParameters,
}
result, err := graphClient.IdentityGovernance().EntitlementManagement().AccessPackageAssignmentRequests().GetWithRequestConfigurationAndResponseHandler(options, nil)


```