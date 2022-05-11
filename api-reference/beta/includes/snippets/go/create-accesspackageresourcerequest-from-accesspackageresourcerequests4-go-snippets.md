---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b8583260c6d0560752b9860e9e3517852060478f
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65323222"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewAccessPackageResourceRequest()
catalogId := "beedadfe-01d5-4025-910b-84abb9369997"
requestBody.SetCatalogId(&catalogId)
requestType := "AdminAdd"
requestBody.SetRequestType(&requestType)
accessPackageResource := msgraphsdk.NewAccessPackageResource()
requestBody.SetAccessPackageResource(accessPackageResource)
originId := "c6294667-7348-4f5a-be73-9d2c65f574f3"
accessPackageResource.SetOriginId(&originId)
originSystem := "AadGroup"
accessPackageResource.SetOriginSystem(&originSystem)
result, err := graphClient.IdentityGovernance().EntitlementManagement().AccessPackageResourceRequests().Post(requestBody)


```