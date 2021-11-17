---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: dda5909b8b30c2f4b9179c6688b342b5bcf00ed9
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "60983111"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestParameters := &msgraphsdk.AccessPackageResourceEnvironmentsRequestBuilderGetQueryParameters{
    Filter: "originSystem%20eq%20'SharePointOnline'",
}
options := &msgraphsdk.AccessPackageResourceEnvironmentsRequestBuilderGetOptions{
    Q: requestParameters,
}
result, err := graphClient.IdentityGovernance().EntitlementManagement().AccessPackageResourceEnvironments().Get(options)


```