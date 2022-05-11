---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: def77a0c3c9056d6d1b83004b299b0fce598921a
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65323224"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewAccessPackageResourceRequest()
catalogId := "26ac0c0a-08bc-4a7b-a313-839f58044ba5"
requestBody.SetCatalogId(&catalogId)
requestType := "AdminAdd"
requestBody.SetRequestType(&requestType)
justification := ""
requestBody.SetJustification(&justification)
accessPackageResource := msgraphsdk.NewAccessPackageResource()
requestBody.SetAccessPackageResource(accessPackageResource)
displayName := "Sales"
accessPackageResource.SetDisplayName(&displayName)
description := "https://contoso.sharepoint.com/sites/Sales"
accessPackageResource.SetDescription(&description)
url := "https://contoso.sharepoint.com/sites/Sales"
accessPackageResource.SetUrl(&url)
resourceType := "SharePoint Online Site"
accessPackageResource.SetResourceType(&resourceType)
originId := "https://contoso.sharepoint.com/sites/Sales"
accessPackageResource.SetOriginId(&originId)
originSystem := "SharePointOnline"
accessPackageResource.SetOriginSystem(&originSystem)
result, err := graphClient.IdentityGovernance().EntitlementManagement().AccessPackageResourceRequests().Post(requestBody)


```