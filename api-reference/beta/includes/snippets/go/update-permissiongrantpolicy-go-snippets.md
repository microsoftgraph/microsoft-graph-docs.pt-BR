---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c6c6a407584a52c2c52cfdfce8e3f1f4a7917a71
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65322285"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewPermissionGrantPolicy()
displayName := "Custom permission grant policy"
requestBody.SetDisplayName(&displayName)
permissionGrantPolicyId := "permissionGrantPolicy-id"
graphClient.Policies().PermissionGrantPoliciesById(&permissionGrantPolicyId).Patch(requestBody)


```