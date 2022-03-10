---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 83db7f225c7db3d537201eb9606b0126774d23dd
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2022
ms.locfileid: "63410992"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewClaimsMappingPolicy()
displayName := "UpdateClaimsPolicy"
requestBody.SetDisplayName(&displayName)
options := &msgraphsdk.ClaimsMappingPolicyRequestBuilderPatchOptions{
    Body: requestBody,
}
claimsMappingPolicyId := "claimsMappingPolicy-id"
result, err := graphClient.Policies().ClaimsMappingPoliciesById(&claimsMappingPolicyId).Patch(options)


```