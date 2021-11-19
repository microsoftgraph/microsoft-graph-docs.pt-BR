---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: baa9bd9c41bca2fc9a72adea86eb8e18f0ce7ca2
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61091487"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewAuthorizationPolicy()
requestBody.SetPermissionGrantPolicyIdsAssignedToDefaultUserRole( []String {
    "managePermissionGrantsForSelf.microsoft-user-default-low",
}
options := &msgraphsdk.AuthorizationPolicyRequestBuilderPatchOptions{
    Body: requestBody,
}
authorizationPolicyId := "authorizationPolicy-id"
graphClient.Policies().AuthorizationPolicyById(&authorizationPolicyId).Patch(options)


```