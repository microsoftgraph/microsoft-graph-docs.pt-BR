---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fae3e290cce9624d5c87f1fa8197200e72de697f
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2022
ms.locfileid: "63410935"
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
result, err := graphClient.Policies().AuthorizationPolicyById(&authorizationPolicyId).Patch(options)


```