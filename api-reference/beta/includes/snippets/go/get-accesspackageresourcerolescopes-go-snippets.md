---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 621a3568049dd20eb1230d059f2f55babe87553f
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "60983796"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestParameters := &msgraphsdk.AccessPackageRequestBuilderGetQueryParameters{
    Expand: "accessPackageResourceRoleScopes($expand=accessPackageResourceRole,accessPackageResourceScope)",
}
options := &msgraphsdk.AccessPackageRequestBuilderGetOptions{
    Q: requestParameters,
}
accessPackageId := "accessPackage-id"
result, err := graphClient.IdentityGovernance().EntitlementManagement().AccessPackagesById(&accessPackageId).Get(options)


```