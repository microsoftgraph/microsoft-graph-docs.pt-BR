---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8f3856f4a3fdaff9ad6a3ee8e96cd5b54212d3c3
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "60983453"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestParameters := &msgraphsdk.AccessPackageAssignmentRequestsRequestBuilderGetQueryParameters{
    Expand: "requestor($expand=connectedOrganization)",
    Filter: "(requestState%20eq%20'PendingApproval')",
}
options := &msgraphsdk.AccessPackageAssignmentRequestsRequestBuilderGetOptions{
    Q: requestParameters,
}
result, err := graphClient.IdentityGovernance().EntitlementManagement().AccessPackageAssignmentRequests().Get(options)


```