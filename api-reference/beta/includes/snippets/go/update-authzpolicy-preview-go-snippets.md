---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 88cabbe39f2a20f3acb2e8c880234aeb7f65344d
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2022
ms.locfileid: "63410934"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewAuthorizationPolicy()
requestBody.SetEnabledPreviewFeatures( []String {
    "assignGroupsToRoles",
}
options := &msgraphsdk.AuthorizationPolicyRequestBuilderPatchOptions{
    Body: requestBody,
}
authorizationPolicyId := "authorizationPolicy-id"
result, err := graphClient.Policies().AuthorizationPolicyById(&authorizationPolicyId).Patch(options)


```