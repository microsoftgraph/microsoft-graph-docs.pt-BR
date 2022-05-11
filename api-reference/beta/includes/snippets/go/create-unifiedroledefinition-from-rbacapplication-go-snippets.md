---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0aa6fedc763a243e7cd4ec04d7eaba008afe6305
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65323863"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewUnifiedRoleDefinition()
description := "Update basic properties of application registrations"
requestBody.SetDescription(&description)
displayName := "Application Registration Support Administrator"
requestBody.SetDisplayName(&displayName)
requestBody.SetRolePermissions( []UnifiedRolePermission {
    msgraphsdk.NewUnifiedRolePermission(),
    SetAdditionalData(map[string]interface{}{
        "allowedResourceActions":  []String {
            "microsoft.directory/applications/basic/read",
        }
    }
}
isEnabled := "true"
requestBody.SetIsEnabled(&isEnabled)
result, err := graphClient.RoleManagement().Directory().RoleDefinitions().Post(requestBody)


```