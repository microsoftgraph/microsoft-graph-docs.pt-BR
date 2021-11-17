---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: febf9ac6ba0ef435519a87a655763bce8bc56d05
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61020688"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewTenantTag()
displayName := "Onboarding"
requestBody.SetDisplayName(&displayName)
description := "Tenants that we are currently onboarding"
requestBody.SetDescription(&description)
options := &msgraphsdk.TenantTagRequestBuilderPatchOptions{
    Body: requestBody,
}
tenantTagId := "tenantTag-id"
graphClient.TenantRelationships().ManagedTenants().TenantTagsById(&tenantTagId).Patch(options)


```