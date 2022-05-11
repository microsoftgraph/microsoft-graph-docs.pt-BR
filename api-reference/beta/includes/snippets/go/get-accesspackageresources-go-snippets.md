---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 169d4bfa781513ac9eb91f1f0b1da431ef9c8da5
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65322628"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.AccessPackageResourcesRequestBuilderGetQueryParameters{
    Filter: "resourceType%20eq%20'Application'",
    Expand: "accessPackageResourceScopes",
}
options := &msgraphsdk.AccessPackageResourcesRequestBuilderGetRequestConfiguration{
    QueryParameters: requestParameters,
}
accessPackageCatalogId := "accessPackageCatalog-id"
result, err := graphClient.IdentityGovernance().EntitlementManagement().AccessPackageCatalogsById(&accessPackageCatalogId).AccessPackageResources().GetWithRequestConfigurationAndResponseHandler(options, nil)


```