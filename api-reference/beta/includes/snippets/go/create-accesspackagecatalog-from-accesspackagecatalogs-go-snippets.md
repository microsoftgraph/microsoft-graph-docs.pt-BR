---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9aaba1273e74337c8850af220e9408cd765de7ef
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61098550"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewAccessPackageCatalog()
displayName := "sales"
requestBody.SetDisplayName(&displayName)
description := "for employees working with sales and outside sales partners"
requestBody.SetDescription(&description)
isExternallyVisible := true
requestBody.SetIsExternallyVisible(&isExternallyVisible)
options := &msgraphsdk.AccessPackageCatalogsRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.IdentityGovernance().EntitlementManagement().AccessPackageCatalogs().Post(options)


```