---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f59a4afaa2e066119814ffb5de4086ca887a5c3b
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2022
ms.locfileid: "63410952"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewAccessReviewPolicy()
isGroupOwnerManagementEnabled := true
requestBody.SetIsGroupOwnerManagementEnabled(&isGroupOwnerManagementEnabled)
options := &msgraphsdk.AccessReviewPolicyRequestBuilderPatchOptions{
    Body: requestBody,
}
result, err := graphClient.Policies().AccessReviewPolicy().Patch(options)


```