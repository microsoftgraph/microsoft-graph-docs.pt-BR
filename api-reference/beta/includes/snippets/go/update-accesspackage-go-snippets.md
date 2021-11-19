---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 98fae05166422e52044419de3701677a4306cbb8
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61082848"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewAccessPackage()
displayName := "Access Package New Name"
requestBody.SetDisplayName(&displayName)
options := &msgraphsdk.AccessPackageRequestBuilderPatchOptions{
    Body: requestBody,
}
accessPackageId := "accessPackage-id"
graphClient.IdentityGovernance().EntitlementManagement().AccessPackagesById(&accessPackageId).Patch(options)


```