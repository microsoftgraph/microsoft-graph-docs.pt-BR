---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bdaa2043660362c5df0ed2cdf68f7b0247c81111
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65322630"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.AccessPackageResourceRolesRequestBuilderGetQueryParameters{
    Filter: "(originSystem%20eq%20'SharePointOnline'%20and%20accessPackageResource/id%20eq%20'53c71803-a0a8-4777-aecc-075de8ee3991')",
    Select: "displayName,originId",
}
options := &msgraphsdk.AccessPackageResourceRolesRequestBuilderGetRequestConfiguration{
    QueryParameters: requestParameters,
}
accessPackageCatalogId := "accessPackageCatalog-id"
result, err := graphClient.IdentityGovernance().EntitlementManagement().AccessPackageCatalogsById(&accessPackageCatalogId).AccessPackageResourceRoles().GetWithRequestConfigurationAndResponseHandler(options, nil)


```