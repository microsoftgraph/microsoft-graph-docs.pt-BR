---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 58c10d790847d172e87195adece957a2a8e00573
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61089581"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewAccessPackageCatalog()
displayName := "Catalog One"
requestBody.SetDisplayName(&displayName)
options := &msgraphsdk.AccessPackageCatalogRequestBuilderPatchOptions{
    Body: requestBody,
}
accessPackageCatalogId := "accessPackageCatalog-id"
graphClient.IdentityGovernance().EntitlementManagement().AccessPackageCatalogsById(&accessPackageCatalogId).Patch(options)


```