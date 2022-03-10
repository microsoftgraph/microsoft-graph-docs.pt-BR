---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fd26620d63b5e3807c04b099d6d461929340a621
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411163"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewCrossTenantAccessPolicy()
displayName := "CrossTenantAccessPolicy"
requestBody.SetDisplayName(&displayName)
options := &msgraphsdk.CrossTenantAccessPolicyRequestBuilderPatchOptions{
    Body: requestBody,
}
result, err := graphClient.Policies().CrossTenantAccessPolicy().Patch(options)


```