---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 13303bf845254e493b365ca7be6a1350945ce172
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65322962"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewAuthorizationPolicy()
defaultUserRolePermissions := msgraphsdk.NewDefaultUserRolePermissions()
requestBody.SetDefaultUserRolePermissions(defaultUserRolePermissions)
defaultUserRolePermissions.SetPermissionGrantPoliciesAssigned( []string {
}
graphClient.Policies().AuthorizationPolicy().Patch(requestBody)


```