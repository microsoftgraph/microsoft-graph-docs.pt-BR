---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 18ce938f41cd811b98630694a78525ad75b78d99
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "60983643"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewAccessPackage()
catalogId := "aa2f6514-3232-46e7-a08a-2411ad8d7128"
requestBody.SetCatalogId(&catalogId)
displayName := "sales reps"
requestBody.SetDisplayName(&displayName)
description := "outside sales representatives"
requestBody.SetDescription(&description)
options := &msgraphsdk.AccessPackagesRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.IdentityGovernance().EntitlementManagement().AccessPackages().Post(options)


```