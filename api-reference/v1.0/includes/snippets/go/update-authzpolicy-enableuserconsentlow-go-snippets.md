---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e934702cb5aeec4e52e4d7bbcc4f3ed799b4e350
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65322963"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewAuthorizationPolicy()
defaultUserRolePermissions := msgraphsdk.NewDefaultUserRolePermissions()
requestBody.SetDefaultUserRolePermissions(defaultUserRolePermissions)
defaultUserRolePermissions.SetPermissionGrantPoliciesAssigned( []String {
    "managePermissionGrantsForSelf.microsoft-user-default-low",
}
graphClient.Policies().AuthorizationPolicy().Patch(requestBody)


```