---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c13e2bc6930891a81a1f2d11995b0e16c6723518
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411061"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewIdentityUserFlowAttribute()
description := "Your new hobby"
requestBody.SetDescription(&description)
options := &msgraphsdk.IdentityUserFlowAttributeRequestBuilderPatchOptions{
    Body: requestBody,
}
identityUserFlowAttributeId := "identityUserFlowAttribute-id"
result, err := graphClient.Identity().UserFlowAttributesById(&identityUserFlowAttributeId).Patch(options)


```